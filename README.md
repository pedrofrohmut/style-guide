# Style Guide for JavaScript ESlint + Prettier + EditorConfig

 Style Guide for React

 A set of rules to facilitate the communication between developers of an react
app.

 Using Prettier to automate the process of formatting and keeping consistence
through out the code base.

Steps:

1 - $ create-react-app <project-name>

2 - $ cd <project-name>

* You can skip Steps 3 and 4 if you have a ESLint configuration file ready to use
that you can copy to your project root

3 - Create and ESLint Configuration File (.eslintrc.json):
  $ npx eslint --init 
  OR
  $ yarn eslint --init

4 - Choose eslint options:
  - How would you like to use ESLint? To check syntax, find problems and enforce
  code style
  - What types of modules your project use? JavaScript Modules (import/esport)
  - Which Framework does your project use? React
  - Where does your code run? browser
  - Would you like to configure ESLint? Use a popular style guide
  - Which style guide to follow? Airbnb
  - What format do config file? JSON
  - Whould you like to install dependencies? Yes (if you are using NPM) No (if not)

  4.1(optional) If you are not using, yarn for example:
    
    You may add prettier as a dev dependency so it can run in other editors without the editor
    plugin dependency.

    Yarn add --dev
	
    ESLINT
      eslint-plugin-react
      eslint-plugin-react-hooks (if you are using hooks)
      eslint-config-airbnb
      eslint-plugin-jsx-a11y
      eslint-plugin-import (optional)
    PRETTIER
      prettier
      eslint-config-prettier
      eslint-plugin-prettier

5 - Add plugins to your editor: 
  VSCode: [Eslint, Prettier, editorconfig]
  VIM: [Ale, editorconfig-vim]

6 - Edit ESLint config file .eslintrc.json
  - Add what you want to overwrite from the defaults from Airbnb

7 - Set Editor options:

  VSCode:
    editor.formatOnSave: true
    prettier.eslintIntegration: true

  Vim (From Prettier Website, :ALEFix):
    let g:ale_fixers = {
    \   'javascript': ['prettier', 'eslint'],
    \   'css': ['prettier'],
    \}
    let g:ale_linters = { 'javascript': ['eslint'] }
    let g:ale_linters_explict = 1
    let g:ale_fix_on_save = 1


8 - Create and edit .editorconfig on the project root (example at this repo rootDir)

9 - Create a .prettierrc to the project root (example at this repo rootDir)

10 - Clean Up the default react app errors and the project is ready to go

