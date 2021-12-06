# blowgraph

This repository contains blowgraph, a graphing library that doesn't suck.

Well, to be fair it doesn't do *anything* yet. But at least it doesn't suck, and that should count for something.

Unfortunately, all popular graphing libraries for Python (matplotlib, pyqtgraph, and everything else) appear to suck beyond measure. You can make pretty pictures in them! Well yes, if you read the source code — because their documentation is atrocious. And once you start reading the source code, it becomes clear that the people who made these libraries just suck at design.

Let's fix that.

## Requirements and desirables

The following is a list of things a properly designed graphing library should be able to do/have:

* Support visualizations of at least 1D and 2D data.
* Support standard, established visualization elements such as axes, colormaps, legends, and so on.
* Support multiple back-ends. The representation of a graph should be renderable to eg. a bitmap, a Qt window, and an SVG file.
* Support for interaction, in backends that support it.
* Graphs that can be updated live, in backends that support it.
* Good performance with large datasets.
* Well-designed low-level OO API with a powerful representation of what a visualisation is.
* Well-designed high-level functions to make it easy to create useful graphs.
* Proper documentation.
* Language independence. But we'll first tackle Python, and once it is stabilized to something decent, we
  may do a re-implementation in C++ or Rust or whatever and make bindings to other languages.
