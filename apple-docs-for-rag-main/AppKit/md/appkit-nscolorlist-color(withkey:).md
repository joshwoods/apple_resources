

- AppKit
- NSColorList
-  color(withKey:) 

Instance Method

# color(withKey:)

Returns the color object associated with the specified key.

macOS

``` source
func color(withKey key: NSColor.Name) -> NSColor?
```

## Parameters 

`key`  

The key for which to retrieve the color.

## Return Value

The color associated with the given key or `nil` if there is none.

## See Also

### Managing Colors By Key

var allKeys: [NSColor.Name]

An array of the keys by which the color objects are stored in the color list.

func insertColor(NSColor, key: NSColor.Name, at: Int)

Inserts the specified color at the specified location in the color list.

func removeColor(withKey: NSColor.Name)

Removes the color associated with the specified key from the color list.

func setColor(NSColor, forKey: NSColor.Name)

Associates the specified color object with the specified key.

