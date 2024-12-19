# monaco-typescript-semantic-token-poc
Proof of concept for supporting better typescript highlighting and semantic tokens in monaco-editor

It's hosted on GitHub pages so you can play with it: https://tspoc.pistonite.dev
You can compare it with the default experience from https://www.typescriptlang.org/play/

## Performance
Range and debounce is implemented. In the hosted example, max length is disabled. You can try
to paste in a very large file (like ts.worker.js from bundled monaco-editor), and enable 6x CPU slow
down in devtool. It should still perform very well.

## Status
I do plan to upstream this. If you like this, please upvote the relevant [issues](https://github.com/microsoft/monaco-editor/issues/2872)/PRs!

- Pending review: Add the tokens to builtin themes: https://github.com/microsoft/vscode/pull/236441 https://github.com/microsoft/vscode/issues/236440
- Pending review: Exposing the Semantic Token API: https://github.com/microsoft/monaco-editor/pull/4788
- TODO: Upstream the modified monarch grammar
- TODO: Upstream the semantic token adapter

## Source
I originally started working on this as part of another project. You can find the source code
[here](https://github.com/Pistonite/botw-ist/tree/215b12ebe9a7efcaabafd9ee1b97f1338521336f/packages/monaco-typescript-contrib/src)

If the patch doesn't get accepted in the upstream, you can reference that to implement it yourself.
