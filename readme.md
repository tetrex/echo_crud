# CRUD REST api's using golang echo-v4


### basic info

creating books libaray CRUD api , to manage books in lib.

```go
 type Book struct {
    name string
    author string
    isbn string
    price int
    qty int
 }
```

- CREATE book [PUT]
    - api to create book
- READ book(s) [GET]
    - api to get array of books
    - isbn?=10,20,30
    - returns []Book
- UPDATE book [PATCH]
    - to update book
    - returns , update status , and updated book
- DELETE book [DELETE] ( soft delete )
    - to delte book
    - return , updated status

### databse

using multiple databases for this project 

- MySQL ( gorm )
- MongoDB

using intercafe model to create generic functions for data update
then using those

primiraly using MongoDB

