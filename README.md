# Config-nuevo-proyecto-Angular

**Nuevo proyecto**

ng new nombre

**Añadir eslint**

ng add @angular-eslint/schematics

**Cambiar karma por jest**

ng add @briebug/jest-schematic

add en jest.config.js
	testPathIgnorePatterns: ["<rootDir>/cypress/"],
	moduleDirectories: [
		".",
		"src",
		"node_modules"
	]
	
*En Ionic:*
	
*Cambiar en angular.json la sección de test.option.assets por "assets": [
      "src/assets"
    ],*

*Borrar el fichero src/test.js*
	
	

**cypress e2e**

ng add @cypress/schematic

cambiar en cypress/integration/spec.ts

cy.contains('nombre de la app app is running!');

**instalar prettier y airbnb para eslint**

npm i -D eslint-config-airbnb-typescript eslint-config-airbnb-base eslint-plugin-import eslint-config-prettier eslint-plugin-prettier prettier

Crear archivo .prettierrc
{
  "singleQuote": true,
  "arrow-body-style": "off",
  "prefer-arrow-callback": "off",
  "printWidth": 120, // optional
  "overrides": [
    {
      "files": "*.html",
      "options": {
        "parser": "html"
      }
    },
    {
      "files": "*.component.html",
      "options": {
        "parser": "angular"
      }
    }
  ]
}

archivo .prettierignore
/dist
/coverage

actualizar .eslintrc.json

extends: 
	"airbnb-typescript/base",
	"prettier"
"plugins": ["prettier", "import"],
rules:
	"import/prefer-default-export": "off",
	"prettier/prettier": "error"	
html 
	extends prettier
	"plugins": ["prettier"],


**test:**

ng test
ng e2e
ng lint


**Material:**
	
ng add @angular/material

**ngx translate**

npm install @ngx-translate/core --save

npm install @ngx-translate/http-loader --save

Config inicial de ngx

**Simple git hooks**

https://github.com/toplenboren/simple-git-hooks
