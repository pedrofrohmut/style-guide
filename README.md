# Style Guide for JavaScript ESlint + Prettier + EditorConfig

 Style Guide for React

 A set of rules to facilitate the communication between the developer of an react
app.

Prettier (extension) to automate the process.

Passos:

1 - $ create-react-app <project-name>

2 - $ cd <project-name>

3 - $ npm install eslint --save-dev

4 - $ npx eslint --init

5 - Choose eslint options:
  - How would you like to use ESLint? To check syntax, find problems and enforce
  code style
  - What types of modules your project use? JavaScript Modules (import/esport)
  - Which Framework does your project use? React
  - Where does your code run? browser
  - Would you like to configure ESLint? Use a popular style guide
  - Which style guide to follow? Airbnb
  - What format do config file? JSON
  - Whould you like to install dependencies? Yes

6 - Add plugins to your editor: [Eslint, Prettier, editorconfig]

7? - Edit ESLint config file .eslintrc.json
  - Add what you want to overwrite from the default from Airbnb

8 - Set Editor options:
  - editor.formatOnSave: true
  - prettier.eslintIntegration: true
  
  * Optional settings:
  "prettier.endOfLine": "lf"
  "prettier.printWidth": 80
  "prettier.semi": false
  "eslint.autoFixOnSave": true
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    { "language": "javascript", "autoFix": true },
    { "language": "javascriptreact", "autoFix": true }
  ]
  "files.trimTrailingWhitespace": true

9 - Create and edit .editorconfig on the project root (example at this repo rootDir)

10 - Enable the plugins, eslint and prettier, and check for errors

11 - Clean Up the default react app errors and the project is ready to go
