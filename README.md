# Setup Eslint with Prettier
### 1. Install Prettier
```
npm install --save-dev prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node
```

### 2. Create .prettierrc file
```
{
  "printWidth": 80,
  "singleQuote": true,
  "trailingComma": "all",
  "bracketSpacing": true,
  "jsxBracketSameLine": false,
  "tabWidth": 4,
  "semi": true
}
```

### 3. Create .eslintrc file
```
{
  "extends": ["react-app", "prettier", "plugin:node/recommended"],
  "rules": {
    "jsx-quotes": [1, "prefer-double"]
  },
  "plugins": ["prettier", "node"]
}

```

### 4. Add File Watcher in Webstorm
Navigate to `WebStorm > Preferences > Tools > File Watchers`
Click on the `+` icon to add a new file watcher. Select `Prettier` template and click `OK`.
Also check that `eslint` is included in the Webstorm.
