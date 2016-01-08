#### Improvements over linter package
 - No DOM operations are performed on panel if it's closed, it's not `hidden` like it used to be, it's completely removed from the document
 - DOM Elements of linter messages are cached as much as possible
 - Messages from all files are not painted on panel and hidden, they are never inserted unless they belong to opened file or showAll option is ticked
 - Messages from the same file are organized in DOM by default
 - Inline bubbles cost a lot less than they used to, they are no longer calculated each time user moves cursor, instead they are counted when messages are inserted

All of these changes combined should improve the linter experience significantly, I hope you like 'em :)