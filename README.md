# etherts

`etherts` is an Ethereum implementation in Typescript. It aims to provide libraries to help dealing with:
- basic cryptography primitives (private key to public key conversion, signature creation and signature verification),
- key management and conversion (between different wallet formats),
- contract ABI encoding/decoding,
- and likely more features.

To achieve some of these goals, it may rely on third party (but proven and well tested) Ethereum Javascript libraries, such as [ethjs] and [ethereumjs], augmenting them with a Typescript definition.

The end goal is to
- provide a developer friendly, but better-than-Javascript, implementation
- be compatible with [AssemblyScript] and as a result with potential [ewasm] contracts

## Why?

Why not just keep improving [ethereumjs]? Good question. Some parts of it have been only patched over the years to keep up with the changes and weren't nicely designed to begin with.
As a result, a lot of code could be rewritten and rewriting in TypeScript gives the added benefit of type security.

[ethjs]: https://github.com/ethjs
[ethereumjs]: https://github.com/ethereumjs
[AssemblyScript]: https://github.com/assemblycsript
[ewasm]: https://github.com/ewasm
