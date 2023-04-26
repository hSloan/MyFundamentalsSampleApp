This is an example DAML implementation of contracts put in place by a Library of Books.

There are 2 types of users:
  1. Librarian
  2. Members

A Librarian can accept Members
A Librarian can add books to the Library's archive
A Member can checkout or return books to an archive

The templates that will need to exist are:  
- `BookArchive` - essentially a Library of Books
- `Books`
- `Members` - users or parties that have signed up to a library

The choices that will need to be in place are:
  1. `AddBook` - add a book to `BookArchive` 
  3. `RequestMembership` - request membership to Library
  4. `ApproveMembership` - approve membership request
  5. `Checkout` - request to checkout a book from `BookArchive`
  6. `Return` - return book that has been checked out from `BookArchive`

Scenarios that are to be tested in this example:
- Only a Librarian should be allowed to add books to a `BookArchive`
- Only Approved Members are allowed to Checkout Books
- Only Books that are available in a `BookArchive` can be checked out
- Only Books that exist in a `BookArchive` and have been checked out can be returned
