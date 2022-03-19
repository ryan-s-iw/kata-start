### Quick Start

Run these commands:
```
npm init -y
npm install --save-dev typescript @types/node jest @types/jest ts-jest ts-node
```

Create tsconfig.json
```
{ // TypeScript configuration file: provides options to the TypeScript 
  // compiler (tsc) and makes VSCode recognize this folder as a TS project,
  // enabling the VSCode build tasks "tsc: build" and "tsc: watch".
  "compilerOptions": {
    "target": "es5",            // Compatible with older browsers
    "module": "umd",            // Compatible with both Node.js and browser
    "moduleResolution": "node", // Tell tsc to look in node_modules for modules
    "sourceMap": true,          // Creates *.js.map files
    "jsx": "react",             // Causes inline XML (JSX code) to be expanded
    "strict": true,             // Strict types, eg. prohibits `var x=0; x=null`
    "alwaysStrict": true        // Enable JavaScript's "use strict" mode
  },
  "include": ["**/*.ts", "**/*.tsx"],
  "exclude": ["node_modules"]
}
```
