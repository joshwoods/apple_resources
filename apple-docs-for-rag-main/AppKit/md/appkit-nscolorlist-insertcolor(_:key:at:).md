

- AppKit
- NSColorList
-  insertColor(\_:key:at:) 

Instance Method

# insertColor(\_:key:at:)

Inserts the specified color at the specified location in the color list.

macOS

``` source
func insertColor(
    _ color: NSColor,
    key: NSColor.Name,
    at loc: Int
)
```

## Parameters 

`color`  

The color to add to the color list.

`key`  

The key with which to associate the color.

`loc`  

The location in the color list at which to place the specified color. Locations are numbered starting with 0.

## Discussion

If the list already contains a color with the same key at a different location, it’s removed from the old location. This method posts didChangeNotification to the default notification center. It raises `NSColorListNotEditableException` if the color list isn’t editable.

## See Also

### Managing Colors By Key

var allKeys: [NSColor.Name]

An array of the keys by which the color objects are stored in the color list.

func color(withKey: NSColor.Name) -> NSColor?

Returns the color object associated with the specified key.

func removeColor(withKey: NSColor.Name)

Removes the color associated with the specified key from the color list.

func setColor(NSColor, forKey: NSColor.Name)

Associates the specified color object with the specified key.

