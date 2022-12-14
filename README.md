# LibraryManagementSystem
// We made these four tables and started designing the login for administrator access

Table: Book

bookID int primary key
bookTitle varchar(50)
publicationYear int
language varchar(10) 
categoryID int
copiesCountActual int
copiesCountCurrent int

Table: BorrowBook

borrowTransactionID string primary key
borrowerID int
bookID int
borrowedFrom date
borrowedTo date
actualReturnDate date
issuedBy int

Table: Staff

staffID int primary key
staffName varchar(50)
password varchar(16)
isAdmin boolean
designation varchar(20)

Table: Student

studentID varchar(12) primary key
studentName varchar(50)
department varchar(10)
borrowerID int
contactNumber varchar(11)