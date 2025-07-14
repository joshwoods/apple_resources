

- AppKit
- NSFormCell
-  titleWidth(\_:) 

Instance Method

# titleWidth(\_:)

Returns the width of the title field constrained to the specified size.

macOS

``` source
@MainActor
func titleWidth(_ size: NSSize) -> CGFloat
```

## Parameters 

`size`  

The maximum size of the field when calculated by the Application Kit.

## Return Value

The width of the title field, measured in points in the user coordinate space.

## Discussion

If you set the width using titleWidth, this method returns the value you set; otherwise, the Application Kit calculates the width, constraining the field size to the specified value.

## See Also

### Related Documentation

var titleWidth: CGFloat

The width of the title field.

