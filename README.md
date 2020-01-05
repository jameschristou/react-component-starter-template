## React Autocomplete Tags Input
A simple React component for displaying an editable list of tags with autocompletion for adding more tags.
This is inspired by the Components field editor in Jira. This component is built using React Hooks and does not
require Redux.

## Features
- Display list of tags and allow user to add and delete tags
- Supply list of allowed tags that user can select from when adding to the list
- Simple interface

### Coming Soon
- Auto versioning and package publish script

## Suggestions & Feature Requests
If you have any suggestions for improvements for feature requests, open an issue on the [github page](https://github.com/jameschristou/react-component-starter-template/issues)

## Installation
The package can be installed via npm
```
npm install my-component
```

### Peer Dependencies
Install the following **peer dependencies** with given versions
```
"react": "^16.10.2",
"react-dom": "^16.10.2"
```

## Usage
- Update the name in package.json to the name of your npm package
- Update the repository urls in package.json
- Update this README
- Use the src folder for your component code
- Replace MyComponent.js with your component
- Replace componentStyle.scss with your component style
- In webpack.component.js replace `output.library` with the name of your component. Also replace entry with the name of your component and its location.
- Build your npm package by running `npm run build:component`
- Publish your component by running `npm publish`

### Default Styling
To include the default styling you will need to import it
```js
import 'my-component/dist-component/style.css';
```

## Development
Run `npm install` to install all packages and depenedencies.

### Dev
To run dev server with HMR while developing use `npm run start`. This will run the project on http://localhost:8080 by default. This will use the test project
in the test folder.

### Build
`npm run build:component`

### Publish
Update the version number of your component and then run `npm publish`

### Analysis
`npm run build:analyze` builds static analysis to examine bundle sizing. You can see output reports in dist/stats.html and dist/report.html
then use http-server to run a http server and access the stats.html. Just run `http-server dist` (ensure you have http-server installed globally)
the dist parameter ensures that it uses the dist folder. It will give you an IP address e.g. http://172.17.126.81:8080 then you can access
stats.html using http://172.17.126.81:8080/stats.html.