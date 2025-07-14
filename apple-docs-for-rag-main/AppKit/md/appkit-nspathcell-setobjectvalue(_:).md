

- AppKit
- NSPathCell
-  setObjectValue(\_:) 

Instance Method

# setObjectValue(\_:)

Sets the receiver’s object value.

macOS 10.5+

``` source
@MainActor
func setObjectValue(_ obj: (any NSCopying)?)
```

## Parameters 

`obj`  

The new object value for the cell.

## Discussion

If `setObjectValue:` is called with an `NSURL` object, clickedPathComponentCell is automatically called. The objectValue method returns the most recently set URL value. The `setObjectValue:` method can also take a string value, with the items separated by the path separator (`/`). Any other value is a programming error and will cause an assertion.

