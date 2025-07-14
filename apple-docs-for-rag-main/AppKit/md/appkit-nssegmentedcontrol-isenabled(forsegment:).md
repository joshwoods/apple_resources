

- AppKit
- NSSegmentedControl
-  isEnabled(forSegment:) 

Instance Method

# isEnabled(forSegment:)

Returns a Boolean value indicating whether the specified segment is enabled.

macOS

``` source
@MainActor
func isEnabled(forSegment segment: Int) -> Bool
```

## Parameters 

`segment`  

The index of the segment whose enabled state you want to get. This method raises an exception (rangeException) if the index is out of bounds.

## Return Value

true if the segment is enabled; otherwise, false.

## See Also

### Enabling and Disabling Segments

func setEnabled(Bool, forSegment: Int)

Sets the enabled state of the specified segment

