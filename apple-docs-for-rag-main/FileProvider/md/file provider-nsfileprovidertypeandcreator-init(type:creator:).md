

- File Provider
- NSFileProviderTypeAndCreator
-  init(type:creator:) 

Initializer

# init(type:creator:)

Creates a structure that contains the provided type and creator codes.

iOS 16.0+iPadOS 16.0+macOS 12.0+visionOS 1.0+

``` source
init(
    type: OSType,
    creator: OSType
)
```

## Parameters 

`type`  

The first word of the `FinderInfo` structure. It matches the file type code.

`creator`  

The second word of the `FinderInfo` structure. It matches the creator code.

## See Also

### Creating Type and Creator Structures

init()

Returns a new type and creator structure with both codes set to `0`.

