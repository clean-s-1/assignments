# Strong tests

[Abstraction and methods for testability](https://github.com/clean-s-1/well-named-in-cpp-hrajpoot-js/pull/1/files)

[Separate formatting from printing](https://github.com/clean-s-1/test-failer-in-js-kmzakiya/blob/ff70ed04625c6730cc4e919ad2583366eb5e6c02/misaligned.js)

## Test the printed manual

Technique for testability = isolate

Isolate the formation of the number and colors -- then the number becomes testable

Isolate the formatting -- then the position of the separator `|` becomes testable

## Hard to test = look for off-the-shelf

Why write code and test the alignment? Why not use tabs (`\t`) instead of `|`?

Why not output comma-separated values (csv), which can be loaded into excel?
