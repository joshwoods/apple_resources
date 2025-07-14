

- AppKit
- NSSegmentedControl
-  label(forSegment:) 

Instance Method

# label(forSegment:)

Returns the label of the specified segment.

macOS

``` source
@MainActor
func label(forSegment segment: Int) -> String?
```

## Parameters 

`segment`  

The index of the segment whose label you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## Return Value

The label of the segment. The returned string contains the entire text of the label, even if that text is normally truncated during drawing.

## See Also

### Configuring the Segment Text

func setLabel(String, forSegment: Int)

Sets the label for the specified segment.

func setAlignment(NSTextAlignment, forSegment: Int)

func alignment(forSegment: Int) -> NSTextAlignment

