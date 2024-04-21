webEngineTopy
========

A toy web rendering engine written in the Rust language forked from Robinson. 

Currently implemented:

* Parse a small subset of HTML and build a DOM tree.
* Parse a small subset of CSS.
* Perform selector matching to apply styles to elements.
* Basic block layout.

Coming soon, I hope:

* Inline layout.
* Paint text and boxes.
* Load resources from network or filesystem.

Instructions
------------

1. [Install Rust 1.0 beta or newer.](http://www.rust-lang.org/install.html)

2. Clone the source code. 

3. Run `cargo build` to build robinson, and `cargo run` to run it.

To build and run with optimizations enabled, use `cargo build --release` and
`cargo run --release`.

By default, robinson will load test.html and test.css from the `examples`
directory.  You can use the `--html` and `--css` arguments to the robinson
executable to change the input files:

    ./target/debug/robinson --html examples/test.html --css examples/test.css

The rendered page will be saved to a file named `output.png`.  To change the
output filename, use the `-o` option.  To switch to PDF output, use add
`--format pdf`.
