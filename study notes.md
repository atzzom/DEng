# data engineering

- how to run an setup a server from the terminal?
- when a server is created, where does it lives in the computer?
- and where is port 5432?
- what's the limit on ports in a/my computer?
- why don't use just port number 1?
- so create a server is just like open the postgres app so the app can take the text ie. queries, and interpret them as sql language?
- if so what part of the program translate or compiles that text into sql code?
- when you create a database or a table, where do they life in the computer?
- database vs schema vs table
- where does localhost lives? and the default ip 127.0.0.1?
- why don't just use the own computer's ip address instead of 127.0.0.1?

- why does a **local** database requires a server service to access the data instead of accessing it just like a regular file in the computer?
even though the data lives in the same computer it is necessary guarantee the following for the data:
| criteria | server | local file |
| 1. concurrency & multi-user access | guarantees concurrent access to the data and multiple users and applications can connect to the data simultaneously | although the data can be accessed by multiple applications at once (who knows if multiple users), this could easily lead to data corruption as there's no mechanism to handle multiple changes made at the same time |
| 2. transaction management | transactions = operations on the data. Servers ensure that each transaction (operation) is either fully completed or not done at all, so data integrity is preserved ie. atomicity with is one of the ACID principles: **A**tomicity, **C**onsistency, **I**solation, **D**urability. | although possible to implement it, it needs consideration of direct (live) file access which is complex and error prone. |

###### 2024-07-09

(today was maintenance day rather than study day)
