<br>

**CHIC602 Project: General Practitioners Project**

<br>

The conda environment is  [`health`](https://github.com/miscellane/indices/tree/develop/development#anaconda-conda)

### Snippets

```
connection = sqlite.connecting(databaseuri='../data/gpinhours.sqlite')
c = connection.cursor()

inhours = c.execute('SELECT * FROM inhours').fetchall()
tables = c.execute("SELECT name FROM sqlite_schema WHERE type = 'table'").fetchall()

c.close()
connection.close()
```
