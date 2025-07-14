

- AppKit
- NSColorPanel
-  detachColorList(\_:) 

Instance Method

# detachColorList(\_:)

Removes the list of colors from all the color pickers in the receiver that display color lists by invoking detachColorList(_:) on all color pickers in the application.

macOS

``` source
@MainActor
func detachColorList(_ colorList: NSColorList)
```

## Parameters 

`colorList`  

The list of `NSColor` objects to remove from the color pickers in the color panel.

## Discussion

Your application should use this method to remove an `NSColorList` saved with a document in its file package or in a directory other than `NSColorList`’s standard search directories.

## See Also

### Managing Color Lists

func attachColorList(NSColorList)

Adds the list of `NSColor` objects specified to all the color pickers in the receiver that display color lists by invoking attachColorList(_:) on all color pickers in the application.

