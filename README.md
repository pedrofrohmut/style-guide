# Style Guide for JavaScript ESlint + Prettier + EditorConfig

 Style Guide for React

 Convenção de regras para facilitar a conversação entre os desenvolvedores detro
de um mesmo projeto.

Prettier para automatizar a aplicação destas regras ao codigo escrito.

Passos:

1 - $ create-react-app <project-name>

2 - $ cd <project-name>

3 - $ npm install eslint --save-dev

4 - $ npx eslint --init

5 - choose eslint options:

  - Would you like to configure ESLINT? Use a popular style guide
  - Which style guide to follow? Airbnb
  - use react? Yes
  - What format do config file? JSON
  - Whould you like to install dependencies? Yes

6 - Add plugins: [Eslint, Prettier, editorconfig]

7? - Edit .eslintrc.json
  - Add what you want to subscribe on the default from Airbnb

8 - Set options:
  - editor.formatOnSave: true
  - prettier.eslintIntegration: true

9 - Create and edit .editorconfig on the project root

10 - Enable the plugins and check for errors

11 - Clean Up react app default errors and the project is ready to go
