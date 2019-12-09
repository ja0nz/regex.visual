# Table of Contents

1.  [Regex Visual WIP](#orgfdee3e3)
    1.  [Technical Overview](#org34b8a54)
    2.  [Roadmap](#orgb625753)


<a id="orgfdee3e3"></a>

# Regex Visual WIP

Think of the [Regex101](https://regex101.com/) but with a different, LISP oriented interface
Based on Oli Savolais ideas: [Regex - a new visual syntax](https://medium.com/interaction-reimagined/regular-expressions-you-can-read-a-new-visual-syntax-526c3cf45df1)


<a id="org34b8a54"></a>

## Technical Overview

I plan to incorporate two regex implementations in form of wasm modules:

1.  [PCRE](https://www.pcre.org/) - the de facto regex standard which already has a [wasm port](https://github.com/desertnet/pcre)
2.  [Rust Regex](https://github.com/rust-lang/regex) - lacking some Regex features but offers linear time execution via a finite-state machine

The main focus of this project will be the interface made by [@thi.ng/umbrella](https://github.com/thi-ng/umbrella/tree/master/examples/crypto-chart).
Not sure yet, but there might be a place for [Parinfer](https://github.com/shaunlebron/parinfer/tree/master/lib) to format the regex human readable.


<a id="orgb625753"></a>

## Roadmap

-   [ ] Compile Rust regex to wasm
-   [ ] Elaborate on the wasm pcre port
-   [ ] Elaborate on parinfer.js
-   [ ] Prototype
