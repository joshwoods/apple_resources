

- AppKit
- NSColorList
-  availableColorLists 

Type Property

# availableColorLists

Returns an array of all color lists found in the standard color list directories.

macOS

``` source
class var availableColorLists: [NSColorList] { get }
```

## Return Value

An array of `NSColorList` objects representing all of the color lists found in the standard color list directories, including color catalogs (lists of colors identified only by name). Color lists created at runtime aren’t included in this list unless they’re saved into one of the standard color list directories.

## See Also

### Getting Lists of Colors

init?(named: NSColorList.Name)

Searches the available color lists array and returns the color list with the specified name.

