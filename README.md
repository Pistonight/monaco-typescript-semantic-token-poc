# monaco-typescript-semantic-token-poc
Proof of concept for supporting better typescript highlighting and semantic tokens in monaco-editor

It's hosted on GitHub pages so you can play with it: https://tspoc.pistonite.dev

## Status
I do plan to upstream this. If you like this, please upvote the relevant issues/PRs!

- Pending review: Add the tokens to builtin themes: https://github.com/microsoft/vscode/pull/236441
- Pending review: Exposing the Semantic Token API: https://github.com/microsoft/monaco-editor/pull/4788
- TODO: Upstream the modified monarch grammar
- TODO: Upstream the semantic token adapter

## Source
I originally started working on this as part of another project. You can find the source code
[here](https://github.com/Pistonite/botw-ist/tree/a510a1b0659f84094f678cddd8c9c3dd24b068f8/packages/monaco-typescript-contrib/src)

If the patch doesn't get accepted in the upstream, you can reference that to implement it yourself.