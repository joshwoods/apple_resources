

- Core Text
- CTRubyAlignment
-  CTRubyAlignment.lineEdge 

Case

# CTRubyAlignment.lineEdge

Aligns the ruby text to an adjacent line edge.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case lineEdge
```

## Discussion

If the ruby text is adjacent to a line edge, Core Text aligns the end of the ruby text adjacent to the line edge to that line edge. This only applies if the width of the ruby text is greater than the width of the base text; otherwise, the alignment is CTRubyAlignment.auto.

If the ruby text isn’t adjacent to a line edge, the alignment is CTRubyAlignment.auto.

## See Also

### Constants

case auto

Core Text automatically determines the alignment.

case start

Aligns the ruby text with the starting edge of the base text.

case center

Centers the ruby text within the width of the base text.

case end

Aligns the ruby text with the ending edge of the base text.

case distributeLetter

Distributes the ruby text evenly over the width of the base text, aligning the first and last characters of the ruby text with the first and last characters of the base text.

case distributeSpace

Distributes the ruby text evenly over the width of the base text, adding space before the first and after the last character.

case invalid

The alignment is invalid.

