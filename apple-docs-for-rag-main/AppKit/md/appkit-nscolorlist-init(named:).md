

- AppKit
- NSColorList
-  init(named:) 

Initializer

# init(named:)

Searches the available color lists array and returns the color list with the specified name.

macOS

``` source
init?(named name: NSColorList.Name)
```

## Parameters 

`name`  

The name of the color list to retrieve. This name must not include the “`.clr`” suffix.

## Return Value

The color list with the specified name or `nil` if no such color list exists.

## See Also

### Related Documentation

var name: NSColorList.Name?

The name of the color list.

### Getting Lists of Colors

class var availableColorLists: [NSColorList]

Returns an array of all color lists found in the standard color list directories.

