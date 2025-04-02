
# Project Structure: API

Let's say we have a project called `applicationA-api` and we want to have a structure that is easy to understand and maintain. Also, some common practices that we want to follow are:

```
applicationA-api/
├── documentation/
├── config/
├── public/
├── scripts/
├── apps/
│   ├── application-1/
|       ├── features/
│           ├── controllers/
│           ├── middlewares/
│           ├── models/
│           ├── routes/
│           ├── services/
│           ├── types/
│           ├── repositories/
│           ├── utils/
│           ├── data-mappers/
│           ├── constants/
│           ├── validators/
│           ├── DTOs/
│           ├── events/
├── packages/
│   ├── package-1/
│       ├── ... 
```

## Detailed Explanation

- `apps/`: The apps of the application, like the API or the web app.
    - `application-1/`: The folder for the application 1 of the application, like the API or the web app.
        - `features/`: The features of the application, like the authentication or the dashboard. This is a common practice in the feature-based architecture. **THIS IS THE MOST IMPORTANT PART OF THE APPLICATION**
            - `controllers/`: The controllers of the application, like the user controller or the product controller.
            - `middlewares/`: The middlewares of the application, like the authentication middleware or the logging middleware.
            - `models/`: The models of the application, like the user model or the product model.
            - `routes/`: The routes of the application, like the user routes or the product routes.
            - `services/`: The services of the application, like the user service or the product service.
            - `types/`: The types of the application, like the user types or the product types.
            - `repositories/`: The repositories of the application, like the user repository or the product repository.
            - `utils/`: The utils of the application, like the helper functions or any other utility function.
            - `data-mappers/`: The data mappers of the application, like the user data mapper or any other data mapper. This is a common practice in DDD (Domain Driven Design).
            - `constants/`: The constants of the application, like any constant that is used in different parts of the application.
            - `validators/`: The validators of the application, like any validator that is used in different parts of the application.
            - `DTOs/`: The DTOs (Data Transfer Objects) of the application, like any DTO that is used in different parts of the application. This is a common practice in DDD (Domain Driven Design).
            - `events/`: The events of the application, like any event that is used in different parts of the application. This is a common practice in DDD (Domain Driven Design).



