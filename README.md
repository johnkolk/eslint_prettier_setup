# Setup Eslint with Prettier
### 1. Install Prettier
```
npm install --save-dev prettier eslint-plugin-prettier eslint-config-prettier
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

### 3. Add File Watcher in Webstorm
Navigate to `WebStorm > Preferences > Tools > File Watchers`
Click on the `+` icon to add a new file watcher. Select `Prettier` template and click `OK`.
Also check that `wslint` is included in the Webstorm.
