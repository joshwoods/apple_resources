

- UIKit
- NSTextSelectionNavigation
- NSTextSelectionNavigation.Destination
-  NSTextSelectionNavigation.Destination.character 

Case

# NSTextSelectionNavigation.Destination.character

The selection moves to the next extended grapheme cluster boundary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
case character
```

## Discussion

When the movement direction isn’t along the line (for example up and down for a horizontal line), it moves to the adjacent line using the anchor point instead of resolving to the logical direction. This could result in a location inside a cluster depending on the specific characteristics of a given script.  For example, certain Indic scripts combine characters in specific ways depending on usage and position to form composite characters. The framework returns a location consistent with the rules of the script and the direction of movement.

## See Also

### Selection destinations

case word

The selection moves to the next word boundary ignoring punctuation, whitespace, and format characters preceding the next word.

case line

The selection moves to the next line boundary.

case sentence

The selection moves to the next sentence boundary, ignoring punctuation, whitespace, and format characters preceding the next sentence.

case paragraph

The selection moves to the next paragraph boundary, ignoring the end of line elastic characters and paragraph separators.

case container

The selection moves to the next container or page boundary after boundary of the current container, ignoring the end of line elastic characters.

case document

The selection moves to the document boundary.

