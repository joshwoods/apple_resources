

- Core Audio Types
- AudioClassDescription
-  init(mType:mSubType:mManufacturer:) 

Initializer

# init(mType:mSubType:mManufacturer:)

Creates an audio class description for the type, subtype, and manufacturer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    mType: OSType,
    mSubType: OSType,
    mManufacturer: OSType
)
```

## Parameters 

`mType`  

A four character code that a manufacturer defines for a codec type.

`mSubType`  

A four character code that a manufacturer defines for a codec subtype.

`mManufacturer`  

A four character code that identifies a codec manufacturer.

## See Also

### Initializers

init()

Creates an empty audio class description.

