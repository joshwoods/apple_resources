

- AppKit
- NSTextSelectionNavigation
- NSTextSelectionNavigation.Destination
-  NSTextSelectionNavigation.Destination.sentence 

Case

# NSTextSelectionNavigation.Destination.sentence

The selection moves to the next sentence boundary, ignoring punctuation, whitespace, and format characters preceding the next sentence.

macOS 12.0+

``` source
case sentence
```

## See Also

### Selection destinations

case character

The selection moves to the next extended grapheme cluster boundary.

case word

The selection moves to the next word boundary ignoring punctuation, whitespace, and format characters preceding the next word.

case line

The selection moves to the next line boundary.

case paragraph

The selection moves to the next paragraph boundary, ignoring the end of line elastic characters and paragraph separators.

case container

The selection moves to the next container or page boundary after boundary of the current container, ignoring the end of line elastic characters.

case document

The selection moves to the document boundary.

