

- AppKit
- NSSegmentedControl
-  setLabel(\_:forSegment:) 

Instance Method

# setLabel(\_:forSegment:)

Sets the label for the specified segment.

macOS

``` source
@MainActor
func setLabel(
    _ label: String,
    forSegment segment: Int
)
```

## Parameters 

`label`  

The label you want to display in the segment. If the width of the string is greater than the width of the segment, the string’s text is truncated during drawing.

`segment`  

The index of the segment whose label you want to set. This method raises an exception (rangeException) if the index is out of bounds.

## See Also

### Configuring the Segment Text

func label(forSegment: Int) -> String?

Returns the label of the specified segment.

func setAlignment(NSTextAlignment, forSegment: Int)

func alignment(forSegment: Int) -> NSTextAlignment

