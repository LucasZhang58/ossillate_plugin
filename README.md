# ossillate_plugin
# A modification of the LSP web extension Example repository (https://github.com/LucasZhang58/vscode-extension-samples/tree/main/lsp-web-extension-sample)
A LSP server that runs in a web extension

## Functionality

This Language Server add color decorators to python files instead of plain text files.

- create a python file
- enter text that contains colors in the format (prrggbb) rather than (#rrggbb)
- color decorators


It also includes an End-to-End test.

## Structure

```
.
├── client // Language Client
│   ├── src
│   │   └── browserClientMain.ts // Language Client entry point
├── package.json // The extension manifest.
└── server // Language Server
    └── src
        └── browserServerMain.ts // Language Server entry point
```

## Running the Sample

- Run `npm install` in this folder. This installs all necessary npm modules in both the client and server folder
- Open VS Code on this folder.
- Press Ctrl+Shift+B to compile the client and server.
- Switch to the Debug viewlet.
- Select `Launch Client` from the drop down.
- Run the launch config.
- If you want to debug the server as well use the launch configuration `Attach to Server`
- In the [Extension Development Host] instance of VSCode, open a document in 'python' language mode.
  - Type p00ff00 or any other color in hex format
  - color decorators will appear

