

- AppKit
- NSColorList
-  removeColor(withKey:) 

Instance Method

# removeColor(withKey:)

Removes the color associated with the specified key from the color list.

macOS

``` source
func removeColor(withKey key: NSColor.Name)
```

## Parameters 

`key`  

The key for which to remove the color.

## Discussion

This method does nothing if the receiver doesn’t contain the key. This method posts didChangeNotification to the default notification center. It raises `NSColorListNotEditableException` if the receiver is not editable.

## See Also

### Managing Colors By Key

var allKeys: [NSColor.Name]

An array of the keys by which the color objects are stored in the color list.

func color(withKey: NSColor.Name) -> NSColor?

Returns the color object associated with the specified key.

func insertColor(NSColor, key: NSColor.Name, at: Int)

Inserts the specified color at the specified location in the color list.

func setColor(NSColor, forKey: NSColor.Name)

Associates the specified color object with the specified key.

