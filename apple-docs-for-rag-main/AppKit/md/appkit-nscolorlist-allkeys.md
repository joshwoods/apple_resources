

- AppKit
- NSColorList
-  allKeys 

Instance Property

# allKeys

An array of the keys by which the color objects are stored in the color list.

macOS

``` source
var allKeys: [NSColor.Name] { get }
```

## See Also

### Managing Colors By Key

func color(withKey: NSColor.Name) -> NSColor?

Returns the color object associated with the specified key.

func insertColor(NSColor, key: NSColor.Name, at: Int)

Inserts the specified color at the specified location in the color list.

func removeColor(withKey: NSColor.Name)

Removes the color associated with the specified key from the color list.

func setColor(NSColor, forKey: NSColor.Name)

Associates the specified color object with the specified key.

