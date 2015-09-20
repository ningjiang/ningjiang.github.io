title: Markdown Syntax
date: 2015-09-20 12:42:58
tags:
---

Examples to demostrate the [markdown syntax](http://daringfireball.net/projects/markdown/syntax).


# INLINE HTML

This is a regular paragraph.

<table>
    <tr>
        <td>Foo</td>
    </tr>
</table>

This is another regular paragraph.


# AUTOMATIC ESCAPING FOR SPECIAL CHARACTERS

http://images.google.com/images?num=30&q=larry+bird

&copy;

AT&T

4 < 5


# HEADERS

This is an H1
=============

This is an H2
-------------

# This is an H1

## This is an H2

###### This is an H6

# This is an H1 #

## This is an H2 ##

### This is an H3 ######


# BLOCKQUOTES

Standard format:

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

Lazy format:

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

Nested format:

> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

Embedded format:

> ## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> Here's some example code:
>
>     return shell_exec("echo $input | $markdown_script");


# LISTS

Asterisks list:

*   Red
*   Green
*   Blue

Pluses list:

+   Red
+   Green
+   Blue

Hyphens list:

-   Red
-   Green
-   Blue

Ordered list:

1.  Bird
2.  McHale
3.  Parish

Lazy ordered list :

1.  Bird
1.  McHale
1.  Parish

Crazy lazy ordered list:

3. Bird
1. McHale
8. Parish

Manual indent list:

*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.

Auto indent list:

*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.

Without blank line:

*   Bird
*   Magic

With blank line:

*   Bird

*   Magic

Multiple paragraphs:

1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.

Lazy multiple paragraphs:

*   This is a list item with two paragraphs.

    This is the second paragraph in the list item. You're
only required to indent the first line. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit.

*   Another item in the same list.

Blockquote within a list item:

*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.

Code block within a list item:

*   A list item with a code block:

        <code goes here>

Unexpected list:

1986. What a great season.

Backslash-escape the period:

1986\. What a great season.


# CODE BLOCKS

This is a normal paragraph:

    This is a code block.

Here is an example of AppleScript:

    tell application "Foo"
        beep
    end tell

HTML code example:

    <div class="footer">
        &copy; 2004 Foo Corporation
    </div>


# HORIZONTAL RULES

Horizontal rule tag:

* * *

- - -

---------------------------------------


# LINKS

URL:

This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.

Local resource:

See my [About](/about/) page for details.

Reference-style links:

This is [an example][id] reference-style link.
This is [an example] [id] reference-style link.

[id]: http://example.com/  "Optional Title Here"

Implicit link:

[Google][]

[Google]: http://google.com/

Visit [Daring Fireball][] for more information.

[Daring Fireball]: http://daringfireball.net/

More example:

I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

[1]: http://google.com/        "Google"
[2]: http://search.yahoo.com/  "Yahoo Search"
[3]: http://search.msn.com/    "MSN Search"

I get 10 times more traffic from [Google][] than from
[Yahoo][] or [MSN][].

[google]: http://google.com/        "Google"
[yahoo]:  http://search.yahoo.com/  "Yahoo Search"
[msn]:    http://search.msn.com/    "MSN Search"


# EMPHASIS

Emphasis:

*single asterisks*

_single underscores_

**double asterisks**

__double underscores__

In the middle of a word:

un*frigging*believable

Backslash escape emphasis:

\*this text is surrounded by literal asterisks\*


# CODE

Span of code:

Use the `printf()` function.

Include backtick character:

``There is a literal backtick (`) here.``

A single backtick in a code span: `` ` ``

A backtick-delimited string in a code span: `` `foo` ``

Include example HTML tags:

Please don't use any `<blink>` tags.

`&#8212;` is the decimal-encoded equivalent of `&mdash;`.


# IMAGES

![Alt text](/path/to/img.jpg)

![Alt text](/path/to/img.jpg "Optional title")

![Alt text][id]

[id]: url/to/image  "Optional title attribute"


# AUTOMATIC LINKS

<http://example.com/>

<address@example.com>


# BACKSLASH ESCAPES

\\literal backslash\\
\`literal backtick\`
\*literal asterisk\*
\_literal underscore\_
\{literal curly braces\}
\[literal square brackets\]
\(literal parentheses\)
\#literal hash mark\#
\+literal plus sign\+
\-literal minus sign (hyphen)\-
\.literal dot\.
\!literal exclamation mark\!
