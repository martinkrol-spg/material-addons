## About

The goal of "material addons" is to achieve a stylesheet similar to [Clarity Addons](https://www.npmjs.com/package/@porscheinformatik/clr-addons) for [Angular Material](https://material.angular.io/).

### Requirements

Material addons requires an already set-up Angular Material project. To do a fresh start please follow [the official Angular Material guide](https://material.angular.io/guide/getting-started) before you continue, but exclude step 4 ("include a theme").

### Installation

1.  Install Material Addons package using npm.

    ```
    npm install @porscheinformatik/material-addons
    ```

2.  Add the stylesheet at the top of your projects styles.scss:

    ```
    @import '~@porscheinformatik/material-addons/themes/styles';
    ```

3.  To use a component, you need to import the Module of the component in your app.module.ts:
    
### Demo

The demo website is linked on the [github repository page](https://github.com/porscheinformatik/material-addons).


### Plan
- [x] Deploy components

- [x] Readonly component

- [x] Action button component

- [x] Toolbar component

- [ ] Use package in Carlos Suite 

- [ ] One navigation entry per component in demo

- [x] Description of development process

- [ ] Issue, pull request templates

- [ ] Use angular material documentation style for examples (cards which enables switching between example and source code)

- [ ] [Storybook?](https://storybook.js.org/docs/guides/guide-angular/)

- [ ] Set up testing

## Development instructions

### Install depenedencies
Install packages via ```npm install```

### Build material addons package
Use ```npm run build:mat-add``` in the [root directory of the material-addons-project](https://github.com/porscheinformatik/material-addons/tree/master/material-addons-project/) to build the package to your local dist directory. 

### Install in demo 
Use ```npm install --no-optional``` to remove old versions of the package in the demo. Afterwards, use normal ```npm install``` to get the newest version of the package from the dist directory.  

### Publish
Use ```npm run publish:mat-add``` to publish a new version on npm. The script bumps the version, builds it and then publishs it to the npm registry. 

### Deploy demo
Use ```npm run deploy:demo``` to deploy a new version to [github pages](https://porscheinformatik.github.io/material-addons) of the demno. 

    


    