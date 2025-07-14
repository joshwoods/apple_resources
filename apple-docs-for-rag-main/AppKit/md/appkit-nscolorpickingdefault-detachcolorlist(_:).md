

- AppKit
- NSColorPickingDefault
-  detachColorList(\_:) 

Instance Method

# detachColorList(\_:)

Tells the receiver to detach the given color list, unless the receiver isn’t displaying the list.

macOS

``` source
@MainActor
func detachColorList(_ colorList: NSColorList)
```

**Required**

## Parameters 

`colorList`  

The color list to detach.

## Discussion

You never invoke this method; it’s invoked automatically by the `NSColorPanel` object when its detachColorList(_:) method is invoked. Because the `NSColorPanel` list mode manages `NSColorList` objects, this method need only be implemented by a custom color picker that manages `NSColorList` objects itself.

## See Also

### Managing Color Lists

func attachColorList(NSColorList)

Tells the receiver to attach the given color list, if it isn’t already displaying the list.

**Required**

