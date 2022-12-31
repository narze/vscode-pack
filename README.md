# VSCode Pack

My extension packs for Visual Studio Code.

## Adding new packs

1. Install Yeoman & `generator-code`

    ```shell
    npm install -g yo generator-code
    ```

1. Bootstrap VSCode extension pack

    ```shell
    yo code
    # Choose "New Extension Pack"
    ```

1. Edit `package.json` -> `extensionPack`

1. Publish

   ```shell
   vsce publish
   ```

## Package & Install as VSIX

```shell
gg && cd python-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix
gg && cd elixir-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix
gg && cd graphql-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix
gg && cd js-ts-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix
gg && cd markdown-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix
gg && cd ruby-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix
gg && cd rust-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix
gg && cd svelte-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix
gg && cd terraform-extension-pack && rm *.vsix && vsce package && code --install-extension *.vsix

# Install all packs
gg && cd narze-extension-packs && rm *.vsix && vsce package && code --install-extension *.vsix
```
