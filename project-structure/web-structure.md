
# Project Structure: Web applications

Let's say we have a project called `applicationA-web` and we want to have a structure that is easy to understand and maintain. Also, some common practices that we want to follow are:

```
applicationA-web/
├── documentation/
├── config/
├── public/
├── scripts/
├── src/
│   ├── pages/
│   ├── services/
│   ├── styles/
│   ├── utils/
│   ├── packages/
│      ├── ui/
│          ├── atoms/
│          ├── molecules/
│          ├── organisms/
│          ├── templates/
│   ├── features/
│       ├── feature-A/
|           ├── components/ 
|           ├── hooks/
|           ├── services
|           ├── types
|
```

## Detailed Explanation

- `src/`: The source code of the application
    - `pages/`: The pages of the application, like the home page or the about page.
    - `services/`: The services of the application, like the API calls or the authentication.
    - `styles/`: The styles of the application, like the CSS or the SCSS files.
    - `utils/`: The utils of the application, like the helper functions or the constants.
    - `packages/`: The packages of the application, like the libraries or the third party packages.
        - `ui/`: The UI components of the application, like the atoms, molecules, organisms and templates. This is a common practice in the atomic design methodology.
            - `atoms/`: The smallest components of the application, like buttons or inputs.
            - `molecules/`: The components that are made up of atoms, like a form or a card.
            - `organisms/`: The components that are made up of molecules, like a header or a footer.
            - `templates/`: The components that are made up of organisms, like a page or a layout.
    - `features/`: The features of the application, like the authentication or the dashboard. This is a common practice in the feature-based architecture. **THIS IS THE MOST IMPORTANT PART OF THE APPLICATION**
        - `feature-A/`: The folder for the feature A of the application, like the authentication or the dashboard.
            - `components/`: The components of the feature A, like the login form or the dashboard.
            - `hooks/`: The hooks of the feature A, like the useAuth hook or the useDashboard hook.
            - `services/`: The services of the feature A, like the API calls or the authentication.
            - `types/`: The types of the feature A, like the types for the API calls or the types for the components.
- `public/`: The public files of the application, like the index.html file
- `config/`: The configuration files of the application, like the env variables or any setting.
- `documentation/`: The documentation of the application, like the README.md file or any other documentation file.
- `scripts/`: The scripts of the application, like the build scripts or any other script that is not part of the source code.


### Component structure

I made the component structure like:

```
project
└─── <component>
    │-  index.ts (required, the provider of the component utilities for the rest of the project)
    │- <component>.tsx (required component file)
    │- <component>.spec.ts (required, in the future)
    │- <component>.module.css (optional)
    │- <component>.types.ts (optional)
    │- <component>.constants.ts (optional)
```


### Detailed Explanation

- `index.ts`: The provider of the component utilities for the rest of the project. This file is required and should export all the utilities that are needed for the component.
- `<component>.tsx`: The component file. This file is required and should contain the component code. Depends of the framework you are using, this file should contain the component code. For example, if you are using React, this file should contain the React component code.
- `<component>.spec.ts`: The test file. This file is required in the future and should contain the tests for the component. This file should be in the same folder as the component file.
- `<component>.module.css`: The CSS file. This file is optional and should contain the styles for the component. This file should be in the same folder as the component file. If you are using a CSS-in-JS library, this file is not needed.
- `<component>.types.ts`: The types file. This file is optional and should contain the types for the component. This file should be in the same folder as the component file. If you are using TypeScript, this file is not needed.
- `<component>.constants.ts`: The constants file. This file is optional and should contain the constants for the component. This file should be in the same folder as the component file. If you are using TypeScript, this file is not needed.
