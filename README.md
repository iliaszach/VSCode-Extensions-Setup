# VSCode-Extensions-Setup
A set of instructions to set up the visual studio code extentions, using only the command line interface.

> ### You only need to do this once, because these extensions will be installed to your Visual Studio Code permantly, until you unistall them

### Step 1: create a new list file in the root of your app:

*echo johnpapa.angular-essentials johnpapa.Angular2 Angular.ng-template	formulahendry.auto-rename-tag esbenp.prettier-vscode eamodio.gitlens bond.better-comments> extensions.list*

**Alternatively, you can use the extensions.list file in this repository, which already includes the suggested extensions.**

### Step 2: Install the extentions via command line interface, with the following command

*for /f "delims=" %i in (extensions.list) do code --install-extension %i*

**Alternatively, if you want to use PowerShell for this operation, you can use the following commad:**

*foreach($line in get-content extensions.list) {code --install-extension $($line)}*

**With the above commands you install the following list of extentions:**

- [Angular Essentials (Version 13)](https://marketplace.visualstudio.com/items?itemName=johnpapa.angular-essentials)
- [Angular Snippets (Version 13)](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)
- [Angular Language Service](https://marketplace.visualstudio.com/items?itemName=Angular.ng-template)
- [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
