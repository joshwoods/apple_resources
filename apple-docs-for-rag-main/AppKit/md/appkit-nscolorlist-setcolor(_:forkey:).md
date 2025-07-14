

- AppKit
- NSColorList
-  setColor(\_:forKey:) 

Instance Method

# setColor(\_:forKey:)

Associates the specified color object with the specified key.

macOS

``` source
func setColor(
    _ color: NSColor,
    forKey key: NSColor.Name
)
```

## Parameters 

`color`  

The color to associate with the given key.

`key`  

The key.

## Discussion

If the list already contains `key`, this method sets the corresponding color to `color`; otherwise, it inserts `color` at the end of the list by invoking insertColor(_:key:at:).

## See Also

### Managing Colors By Key

var allKeys: [NSColor.Name]

An array of the keys by which the color objects are stored in the color list.

func color(withKey: NSColor.Name) -> NSColor?

Returns the color object associated with the specified key.

func insertColor(NSColor, key: NSColor.Name, at: Int)

Inserts the specified color at the specified location in the color list.

func removeColor(withKey: NSColor.Name)

Removes the color associated with the specified key from the color list.

