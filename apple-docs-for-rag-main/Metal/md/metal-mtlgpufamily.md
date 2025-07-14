

- Metal
-  MTLGPUFamily 

Enumeration

# MTLGPUFamily

Represents the functionality for families of GPUs.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum MTLGPUFamily
```

## Mentioned in 

Detecting GPU Features and Metal Software Versions

Improving your game’s graphics performance and settings

## Overview

Check whether a GPU supports the features of a specific family by calling the supportsFamily(_:) method of a GPU’s MTLDevice instance.

## Topics

### Checking for Common GPU Support

case metal3

Represents the Metal 3 features.

case common3

Represents the Common family 3 GPU features.

case common2

Represents the Common family 2 GPU features.

case common1

Represents the Common family 1 GPU features.

### Checking for Apple Family GPU Support

case apple9

Represents the Apple family 9 GPU features that correspond to the Apple A17, M3, and M4 GPUs.

case apple8

Represents the Apple family 8 GPU features that correspond to the Apple A15, A16, and M2 GPUs.

case apple7

Represents the Apple family 7 GPU features that correspond to the Apple A14 and M1 GPUs.

case apple6

Represents the Apple family 6 GPU features that correspond to the Apple A13 GPUs.

case apple5

Represents the Apple family 5 GPU features that correspond to the Apple A12 GPUs.

case apple4

Represents the Apple family 4 GPU features that correspond to the Apple A11 GPUs.

case apple3

Represents the Apple family 3 GPU features that correspond to the Apple A9 and A10 GPUs.

case apple2

Represents the Apple family 2 GPU features that correspond to the Apple A8 GPUs.

case apple1

Represents the Apple family 1 GPU features that correspond to the Apple A7 GPUs.

### Checking for macOS Family GPU Support

case mac2

Represents the Mac family 2 GPU features.

case mac1

Represents the Mac family 1 GPU features.

Deprecated

### Checking for Mac Catalyst Family GPU Support

case macCatalyst2

Represents a family 2 Mac GPU when running an app you built with Mac Catalyst.

Deprecated

case macCatalyst1

Represents a family 1 Mac GPU when running an app you built with Mac Catalyst.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking a GPU Device’s Feature Support

func supportsFamily(MTLGPUFamily) -> Bool

Returns a Boolean value that indicates whether the GPU device supports the feature set of a specific GPU family.

**Required**

func supportsFeatureSet(MTLFeatureSet) -> Bool

Returns a Boolean value that indicates whether the GPU device supports a specific feature set.

**Required**

Deprecated

enum MTLFeatureSet

The device feature sets that define specific platform, hardware, and software configurations.

Deprecated

