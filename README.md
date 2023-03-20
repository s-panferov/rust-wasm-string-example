
An example of a small text-heavy Rust application. Created to demonstrate how much time text decoding takes.

Strings are extracted from the https://tailwindui.com/components?ref=sidebar page with this script:

```js
Array.from(document.body.querySelectorAll("*")).map(n => Array.from(n.attributes).map(a => a.nodeValue)).flat()
```

To run the example use Rust + [Trunk](https://trunkrs.dev/)

```rust
trunk serve --release
``