# python-connection-pooling

This shows off how to use connection pooling in Python with Dolt

# Setup

1. Make a Dolt database with a single table test
```
$ mkdir test_python_connection_pool
cd test_python_connection_pool 
$ dolt init --fun
Successfully initialized dolt data repository.
 test (pk int, c1 int, primary key(pk))"
$ dolt sql-server
```

2. Run the test.py script
```
$ python test.py
Reading an uncommitted transaction. Will show empty.
[]
Reading off transaction begun when pool was made. Will show empty.
[]
Will show new row.
[(0, 0)]
Will show two rows.
[(0, 0), (1, 1)]
```
