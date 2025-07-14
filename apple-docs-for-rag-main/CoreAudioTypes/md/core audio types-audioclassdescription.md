

- Core Audio Types
-  AudioClassDescription 

Structure

# AudioClassDescription

A structure that describes an audio codec.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioClassDescription
```

## Topics

### Accessing the Data

var mType: OSType

A four character code that a manufacturer defines for a codec type.

var mSubType: OSType

A four character code that a manufacturer defines for a codec subtype.

var mManufacturer: OSType

A four character code that identifies a codec manufacturer.

### Initializers

init()

Creates an empty audio class description.

init(mType: OSType, mSubType: OSType, mManufacturer: OSType)

Creates an audio class description for the type, subtype, and manufacturer.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

