# Book-API-2.0
Update of version 1.0 | Java RMI | codebase

In version 1.0, we have some issues. In this new version, we are going to tackle it. The following is the problems we encounted.

## Problem
Book class must availble in client side (this is a problem!)

Instance of class BookShelf is used through registry server and method getBook() return a Book class. Book class implements Serialization interface so that a book instance be able to be send throw socket.

Give client entire code of Book class is catastrophic. Client will know how your Book class work, it like a leak infomation. Therefore, perharps, client can buld their own service. As a result, you lost code as well as client.




