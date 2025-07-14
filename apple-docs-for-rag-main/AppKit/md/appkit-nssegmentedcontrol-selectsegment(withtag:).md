

- AppKit
- NSSegmentedControl
-  selectSegment(withTag:) 

Instance Method

# selectSegment(withTag:)

Selects the segment with the specified tag.

macOS

``` source
@MainActor
func selectSegment(withTag tag: Int) -> Bool
```

## Parameters 

`tag`  

The tag associated with the desired segment. A tag is an integer value that can be assigned to a segment as a way of identifying it without knowing its position in the control.

## Return Value

true if the segment was selected successfully; otherwise, false.

## Discussion

Typically, you use Interface Builder to specify the tag for each segment. You may also set this value programmatically using the `setTag:forSegment:` method of `NSSegmentedCell`.

## See Also

### Related Documentation

func setTag(Int, forSegment: Int)

Sets the tag for the specified segment.

### Managing the Selected Segment

var selectedSegment: Int

The index of the selected segment of the control, or `-1` if no segment is selected.

var indexOfSelectedItem: Int

func setSelected(Bool, forSegment: Int)

Sets the selection state of the specified segment.

func isSelected(forSegment: Int) -> Bool

Returns a Boolean value indicating whether the specified segment is selected.

var selectedSegmentBezelColor: NSColor?

The color of the selected segment’s bezel, in appearances that support it.

var doubleValueForSelectedSegment: Double

When the tracking mode for the control is set to use a momentary accelerator, returns a value for the selected segment.

