# Architecture decisions

## For the applications in general

### Feature Folder

We want to use a `feature` folder to contain all the business logic of the application. This is a common practice in the feature-based architecture. The folder should contain all the components, hooks, services, types and any other file that is related to the feature. This way we can have a clear separation of concerns and we can easily find the files that are related to the feature.


### Config folder

We want to use this to handle the env variables and any config information of the application.

### Documentation folder

We want to use this to handle the documentation of the application. Any information related to the database, or the design or the UI/UX. We want to use **design docs** to enhance the traceability of the features and the decisions that we make.

For the design docs we want to use a template that I'm going to upload on this repository


## For the API

We want to use the monorepo architecture to handle the different applications that we have. This way we can have a clear separation of concerns and we can easily find the files that are related to the application.

In this context we're going to use:
- `apps` folder: to handle the different applications that we have. This way we can have a clear separation of concerns and we can easily find the files that are related to the application.
- `packages` folder: to handle the different packages that we have. For example to use an ORM library, or a fetching library or a time library. We want to abstract the logic of the library and use it in the application.


## For the web applications

We want to use the atomic design methodology to handle the different components that we have. This way we can have a clear separation of concerns and we can easily find the files that are related to the component.

Also, we want to use the monorepo architecture to handle the different applications that we have. This way we can have a clear separation of concerns and we can easily find the files that are related to the application.


In this context we're going to use:
- `packages` folder: to handle the different internal libraries that we have. For example each project it's going to have a base UI library made with our technologies or maybe we can use another one and adapt it to our project. So on this folder we can have the components that we're going to use on the application



