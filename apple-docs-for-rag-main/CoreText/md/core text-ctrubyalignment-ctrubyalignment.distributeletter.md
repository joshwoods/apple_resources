

- Core Text
- CTRubyAlignment
-  CTRubyAlignment.distributeLetter 

Case

# CTRubyAlignment.distributeLetter

Distributes the ruby text evenly over the width of the base text, aligning the first and last characters of the ruby text with the first and last characters of the base text.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case distributeLetter
```

## Discussion

If the width of the ruby text is less than the width of the base text, Core Text evenly distributes the ruby text over the width of the base text. The first character of the ruby text aligns with the first character of the base text, and the last character of the ruby text aligns with the last character of the base text.

If the width of the base text is less than the width of the ruby text, Core Text evenly distributes the base text over the width of the ruby text.

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

case distributeSpace

Distributes the ruby text evenly over the width of the base text, adding space before the first and after the last character.

case lineEdge

Aligns the ruby text to an adjacent line edge.

case invalid

The alignment is invalid.

