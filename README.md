# TodoApp
React Todo Application using CI/CD

1. Create react app
``` 
    npx create-react-app todoapp
```
2. Build react project
```
    npm run build
```
You can view todoapp in the browser at: http://localhost:3000

3. Init Github page
```
    npm install gh-pages --save-dev
```
Config package.json (homepage, predeploy, and deploy) such as:
```
  "name": "todoapp",
  "homepage": "https://cuonganh.github.io/todoapp",
  "version": "0.1.0",
  "private": true,
  "dependencies": {
    "@testing-library/jest-dom": "^5.16.5",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-scripts": "5.0.1",
    "web-vitals": "^2.1.4"
  },
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  }
```
4. Deploy react app
```
    npm run deploy
```
After that, you can try your react app at https://cuonganh.github.io/todoapp/