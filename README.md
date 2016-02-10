cse stands for context-sensitive escaping
========================================

context stands for the parser state when
parsing a HTML document.


escaping stands for replacing characters
so that templating input does not modify
the current context.


Example:

`var foo = \`<a href="${foo}">click me</a>\``


If you want to escape `foo` in a context-sensitive
way you need to make sure that, the parser will remain
in the "a element, href attribute" state when the input
has been processed
