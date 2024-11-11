# SPREAD Vale package

This repo contains the vale package for linting SPREAD language. The package is built on the Microsoft Style Guide.

## Language linting using Vale

![An image of Vale inside Visual Studio Code](https://docs.spread.ai/src/vale-inside-vscode-1280x800.png)

Vale is a lightweight writing tool that checks your writing for errors, and suggests fixes for better technical writing. We use Vale in the publish pipeline for creating our documentation, so it makes sense that you use it too when creating documentation. To enable Vale in Visual Studio Code:

1. Copy this repository into your project's repository and rename it `docs`. Make sure that it is a top-level directory.

2. Install the Vale CLI: `brew install vale`

3. Inside Visual Studio Code, install the [Vale-VSCode](https://marketplace.visualstudio.com/items?itemName=ChrisChinchilla.vale-vscode) extension.

4. Select **Code** > **Settings** > **Settings** or use the **⌘**-**,** shortcut to open Settings.

5. Select **Extensions** in the right-hand side menu and then select **Vale**. In the **Vale > Vale CLI: Config** field enter: `/Users/YOUR_USER_NAME/.../docs-template/.vale.ini`. Make sure to replace YOUR_USER_NAME with your user name and to replace the ellipsis with the path to the repository.

![An image of Vale inside Visual Studio Code](src/vale-extension-setting-1974x468.png)

6. In the **Vale > Vale CLI: Path** field enter: `/opt/homebrew/bin/vale`

6. Inside the `docs` directory run the following command in your terminal or console: `vale sync`

7. Restart Visual Studio Code and start writing your content. Errors and suggestions will appear as you are writing.

For instructions on how to use Vale with JetBrains, see [JetBrains Integration](https://vale.sh/docs/integrations/jetbrains/) in the Vale Documentation.

