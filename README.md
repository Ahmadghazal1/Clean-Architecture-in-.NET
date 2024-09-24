# Clean-Architecture-in-.NET
Clean Architecture Solution Template 


### What is Clean Architecture?
Clean Architecture is an architecture pattern aimed at building applications that we can maintain, scale, and test easily.


###[1].Domain Layer :
The domain layer represents the application’s core business rules and entities. This is the innermost layer and should not have any external dependencies.

###[2].Application Layer :
The application layer sits just outside the domain layer and acts as an intermediary between the domain layer and other layers. In other words, it contains the use cases of the application and we expose the core business rules of the domain layer through the application layer. This layer depends just on the domain layer.

###[3].Infrastructure Layer :
We implement all the external services like databases, file storage, emails, etc. in the infrastructure layer. It contains the implementations of the interfaces defined in the domain layer.

###[4].Presentation Layer :
The presentation layer handles the user interactions and fetches data to the user interface.
