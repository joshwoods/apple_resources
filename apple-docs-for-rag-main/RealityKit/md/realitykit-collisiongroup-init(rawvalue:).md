

- RealityKit
- CollisionGroup
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a collision group from a raw value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init(rawValue: UInt32)
```

## Parameters 

`rawValue`  

The raw value of the option set to create. Each bit of rawValue potentially represents an element of the option set, though raw values may include bits that are not defined as distinct values of the OptionSet type.

## Discussion

This initializer succeeds even if the value passed as `rawValue` exceeds the static properties declared as part of the option set. Usually, you will want to create each collision groups setting a different bit flag for each value, so that multiple individual groups can be combined using OptionSet methods.

Here is an example of creating four collision groups using different bitflag values for each one.

```
let redGroup = CollisionGroup(rawValue: 1 

## See Also

### Creating a collision group

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

