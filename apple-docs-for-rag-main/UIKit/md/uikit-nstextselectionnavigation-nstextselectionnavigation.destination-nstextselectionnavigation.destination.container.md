

- UIKit
- NSTextSelectionNavigation
- NSTextSelectionNavigation.Destination
-  NSTextSelectionNavigation.Destination.container 

Case

# NSTextSelectionNavigation.Destination.container

The selection moves to the next container or page boundary after boundary of the current container, ignoring the end of line elastic characters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
case container
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

case paragraph

The selection moves to the next paragraph boundary, ignoring the end of line elastic characters and paragraph separators.

case document

The selection moves to the document boundary.

