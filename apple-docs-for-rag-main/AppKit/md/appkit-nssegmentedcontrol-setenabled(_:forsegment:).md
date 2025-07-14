

- AppKit
- NSSegmentedControl
-  setEnabled(\_:forSegment:) 

Instance Method

# setEnabled(\_:forSegment:)

Sets the enabled state of the specified segment

macOS

``` source
@MainActor
func setEnabled(
    _ enabled: Bool,
    forSegment segment: Int
)
```

## Parameters 

`enabled`  

true to enable the segment; otherwise, false to disable it.

`segment`  

The index of the segment you want to enable or disable. This method raises an exception (rangeException) if the index is out of bounds.

## See Also

### Enabling and Disabling Segments

func isEnabled(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is enabled.

