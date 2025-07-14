

- AppKit
- NSColorPanel
-  attachColorList(\_:) 

Instance Method

# attachColorList(\_:)

Adds the list of `NSColor` objects specified to all the color pickers in the receiver that display color lists by invoking attachColorList(_:) on all color pickers in the application.

macOS

``` source
@MainActor
func attachColorList(_ colorList: NSColorList)
```

## Parameters 

`colorList`  

The list of colors to add to the color pickers in the receiver.

## Discussion

An application should use this method to add an `NSColorList` saved with a document in its file package or in a directory other than `NSColorList`’s standard search directories.

## See Also

### Managing Color Lists

func detachColorList(NSColorList)

Removes the list of colors from all the color pickers in the receiver that display color lists by invoking detachColorList(_:) on all color pickers in the application.

