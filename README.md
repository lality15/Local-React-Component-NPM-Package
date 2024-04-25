Documentation: Setting Up a React Project with Babel

Create Directory:
Use the command mkdir directoryName to create a directory for your project.
Navigate to Directory:
Change directory to directoryName using the command cd directoryName.
Initialize npm:
Run npm init to initialize a new npm package.json file. Follow the prompts and press 'y' to confirm.
Install Babel:
Install Babel and its core dependencies using the command:
npm install @babel/cli @babel/core --save-dev
Install Babel Presets:
npm install @babel/preset-env @babel/preset-react --save-dev
Create .babelrc File:
{
  "presets": ["@babel/preset-env", "@babel/preset-react"]
}
Create Source Directory:
Within directoryName, create a directory named src.
Create React Component:
Inside the src directory, create a file xyz.js.
import React from 'react';

export default function DisplayName() {
    return (
        <div>
            <h1>Hello Lalit</h1>
        </div>
    );
}
Compile with Babel:
Open the CLI and use pwd to get the project's path.
Run the following command to compile the code:
babel src --out-file xyz.js
Update package.json Scripts:
Open package.json and add the following script :
"scripts": {
  "build": "babel src --out-file xyz.js"
}
Build Using npm:
Execute the following command in the CLI:
npm run build
Install React Dependencies:
Install React and ReactDOM:
npm install react react-dom --save-dev
Create React App:
Use npx create-react-app app-name to create a new React app.
Install Custom Package:
Navigate to the React app directory and install your custom package using:
npm install path_to_the_package Like npm install ../Package-Name

