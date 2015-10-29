TapDigit is a playground for JavaScript implementation of math-related code, such as expression lexer/parser, evaluator, and so on.

**TapDigit.Lexer** is a simple lexical scanner which splits a math expression into a sequence of _tokens_. This is useful for color-highlighted expression editor.

TapDigit has an HTML-based editor (with JavaScript-implementation of the editing logic) ready to use as **TapDigit.Editor** object, as illustrated in this screenshot:

![https://lh3.googleusercontent.com/-34e-mQdsggU/TiZfM2AxihI/AAAAAAAACAg/yUMBjx4iJwY/s800/tapdigit-editor.png](https://lh3.googleusercontent.com/-34e-mQdsggU/TiZfM2AxihI/AAAAAAAACAg/yUMBjx4iJwY/s800/tapdigit-editor.png)

**TapDigit.Parser** takes an expression and produces JSON-formatted syntax tree representation thereof.

**TapDigit.Evaluator** computes the result of an expression. Variables, constants, and functions supported in the expression syntax can be extended via **TapDigit.Context** object.

For more information, check the [summary of features](Overview.md), explore [the source code](http://code.google.com/p/tapdigit/source/checkout), and [try it live](http://tapdigit.googlecode.com/git/demo.htm).

TapDigit is created by [Ariya Hidayat](http://ariya.ofilabs.com). Follow me on Twitter [@ariyahidayat](http://twitter.com/AriyaHidayat) to get fresh updates.