# PythonTips
Raymond Hettinger

combine a list of lists into a single set
```python
lol = [['a', 'b', 'c'], ['b', 'c', 'd'], ['d', 'e']]
set().union(*lol)
set(['a', 'c', 'b', 'e', 'd'])
```

The csv module can "sniff" unknown CSV dialects:
```python
with open('example.csv', 'rb') as csvfile:
    dialect = csv.Sniffer().sniff(http://csvfile.read (1024))
    http://csvfile.seek (0)
    reader = csv.reader(csvfile, dialect)\
```

Adding %(filename)s and %(lineno)d to the logging format makes it easier to see where log messages came from.
