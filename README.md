# 💅 My Prettier config

### 💡 Motivation
I created and publish this package to npm so I can use the same configuration across all my personal projects.

### 💻 Installation
Using npm `npm i --save-dev @qsalatiel/prettier-config`
Using yarn `yarn add -D @qsalatiel/prettier-config`

### How to use it

**Via package file**
You can add `"prettier": "@qsalatiel/prettier-config"` to your `package.json`

**Via prettierrc file**
Create a `.prettierrc.json` file with `"@qsalatiel/prettier-config"`

**Via .prettierrc.js if you want to override it**
Create a `.prettierrc.js` file and add the following content:
```javascript
module.exports = {
	...require("@qsalatiel/prettier-config"),
	semi: false,
};
```

### 👀 What this config looks like:

```json
{
  "printWidth": 100,
  "tabWidth": 2,
  "useTabs": false,
  "semi": false,
  "singleQuote": true,
  "trailingComma": "es5",
  "bracketSpacing": true,
  "jsxBracketSameLine": false,
  "arrowParens": "avoid",
  "overrides": [
    {
      "files": "*.css",
      "options": {
        "singleQuote": false,
        "parser": "css"
      }
    }
  ]
}
```