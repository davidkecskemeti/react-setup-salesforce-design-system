# Salesforce setup react app

1. Create a new app
   - `create-react-app my-react-app`
1. Install NPM modules
   - `cd my-react-app && npm install @salesforce-ux/design-system @salesforce/design-system-react`
1. Copy SLDS CSS file to `public` folder
   - `cp node_modules/@salesforce-ux/design-system/assets/styles/salesforce-lightning-design-system.min.css public/`
1. Copy SLDS icons folder to `public` folder
   - `cp -r node_modules/@salesforce-ux/design-system/assets/icons public/`
1. Copy SLDS fonts folder to `public` folder
   - `cp -r node_modules/@salesforce-ux/design-system/assets/fonts public/`
1. Add CSS file to `index.html`
   - `<link rel="stylesheet" type="text/css" href="/salesforce-lightning-design-system.min.css">`

### Ready to GO

### Import components

- `import { Button, IconSettings } from '@salesforce/design-system-react';`

### Modify the `iconPath` prop of `IconSettings` to output the correct path to the icons in the public folder.

- `<IconSettings iconPath="/icons">{// doc site examples}</IconSettings>`
