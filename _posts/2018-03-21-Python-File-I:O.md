---
layout: post
title: Python File I/O
---

Just for reminding. 
## pickle
The easiest way is to use pickle, it can support all kinds of data formats, list & dict.  
```python
import pickle
test = [1, 2, 3, 4]
# write
with open('test.txt', 'wb') as fp:
    pickle.dump(test, fp)
# read
with open('test.txt', 'rb') as fp:
    read_test = pickle.load(fp)
print(read_test)
# [1, 2, 3, 4]
```
The problem with pickle is that the output file needs to be opened in binary mode. The following code will output an error. So the file is not readable using text edit tool. 
```python
with open('test.txt', 'w') as fp:
    pickle.dump(test, fp)
```
## json
While, the json library can do the same work with readable output file. 
```python
import json
data = {"a": 1, "b": 2, "c": 3}
# write
with open('test.txt', 'w') as fp:
    json.dump(data, fp)
# read
with open('test.txt', 'r') as fp:
    data = json.load(fp)
print(data)
# {'a': 1, 'b': 2, 'c': 3}
```

### Write and read list to txt file
```python
# write one item a line
with open('test.txt', 'w') as fp:
    for item in test:
        fp.write('%s\n' % item)
# read
with open('test.txt', 'r') as fp:
    read_test = fp.read().splitlines()
print(read_test)
# ['1', '2', '3', '4']
```
Note that the element in read_test is a string type, you may need to convert it back to Integer or other formats. 
```python
read_test = list(map(int, read_test))
```

### write and read list of list to csv file
```python
import csv
test = [[1, 2, 3], [4, 5, 6]]
# write
with open('test.csv', 'w') as fp:
    wr = csv.writer(fp)
    wr.writerows(test)
# read
with open('test.csv', 'r') as fp:
    read_test = [rec for rec in csv.reader(fp)]
print(read_test)
# [['1', '2', '3'], ['4', '5', '6']]
```

