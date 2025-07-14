

- AppKit
- NSTextSelectionNavigation
- NSTextSelectionNavigation.Destination
-  NSTextSelectionNavigation.Destination.paragraph 

Case

# NSTextSelectionNavigation.Destination.paragraph

The selection moves to the next paragraph boundary, ignoring the end of line elastic characters and paragraph separators.

macOS 12.0+

``` source
case paragraph
```

## See Also

### Selection destinations

case character

The selection moves to the next extended grapheme cluster boundary.

case word

The selection moves to the next word boundary ignoring punctuation, whitespace, and format characters preceding the next word.

case line

The selection moves to the next line boundary.

case sentence

The selection moves to the next sentence boundary, ignoring punctuation, whitespace, and format characters preceding the next sentence.

case container

The selection moves to the next container or page boundary after boundary of the current container, ignoring the end of line elastic characters.

case document

The selection moves to the document boundary.

