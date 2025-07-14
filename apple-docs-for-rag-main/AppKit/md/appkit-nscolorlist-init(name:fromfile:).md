

- AppKit
- NSColorList
-  init(name:fromFile:) 

Initializer

# init(name:fromFile:)

Initializes and returns a color list from the specified file, registering it under the specified name if it isn’t in use already.

macOS

``` source
init?(
    name: NSColorList.Name,
    fromFile path: String?
)
```

## Parameters 

`name`  

The name of the file for the color list (minus the `“.clr”` extension). Specify `@””` if you don’t want a name.

`path`  

The full path to the file for the color list. A `nil` path indicates the color list should be initialized with no colors.

## Discussion

Note that this method does not add the color list to availableColorLists until the color list is saved into the user’s path with write(toFile:) with a value of `nil`.

## See Also

### Creating Lists of Colors

init(name: NSColorList.Name)

Initializes and returns a color list, registering it under the specified name if it isn’t in use already.

