

- AppKit
- NSColorList
-  init(name:) 

Initializer

# init(name:)

Initializes and returns a color list, registering it under the specified name if it isn’t in use already.

macOS

``` source
init(name: NSColorList.Name)
```

## Parameters 

`name`  

The name under which to register the color list. Specify `@””` if you don’t want a name.

## Return Value

The initialized color list.

## Discussion

This method invokes init(name:fromFile:) with a `fromFile:` argument of `nil`, indicating that the color list doesn’t need to be initialized from a file. Note that this method does not add the color list to availableColorLists until the color list is saved into the user’s path with write(toFile:) with a value of `nil`.

## See Also

### Related Documentation

Color Programming Topics

### Creating Lists of Colors

init?(name: NSColorList.Name, fromFile: String?)

Initializes and returns a color list from the specified file, registering it under the specified name if it isn’t in use already.

