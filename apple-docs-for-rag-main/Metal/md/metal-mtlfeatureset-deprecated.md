

- Metal
-  MTLFeatureSet Deprecated

Enumeration

# MTLFeatureSet

The device feature sets that define specific platform, hardware, and software configurations.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum MTLFeatureSet
```

Deprecated

Use MTLGPUFamily instead.

## Overview

If your app is running on an operating system that supports the supportsFamily(_:) method, use that method instead. See Detecting GPU Features and Metal Software Versions for more information about MTLGPUFamily — the replacement for this enumeration —  and the feature set tables. This type doesn’t define constants for GPU families introduced after iOS GPU family 5.

Metal feature sets define the feature availability, implementation limits, and pixel format capabilities for each device. The table shows the GPU families and their corresponding GPU hardware.

| GPU family | GPU hardware |
|----|----|
| iOS GPU family 1 | Apple A7 devices |
| iOS GPU family 2  tvOS GPU family 1 | Apple A8 devices |
| iOS GPU family 3  tvOS GPU family 2 | Apple A9 devices  Apple A10 devices |
| iOS GPU family 4 | Apple A11 devices |
| iOS GPU family 5 | Apple A12 devices |
| macOS GPU family 1 | iMac Pro models  iMac models from 2012 or later  MacBook models from 2015 or later  MacBook Pro models from 2012 or later  MacBook Air models from 2012 or later  Mac mini models from 2012 or later  Mac Pro models from late 2013 |
| macOS GPU family 2 | iMac models from 2015 or later  MacBook Pro models from 2016 or later  MacBook models from 2016 or later  iMac Pro models from 2017 or later |

For more information on Mac support for Metal, see Mac computers that support Metal.

## Topics

### iOS GPU Family 5

case iOS_GPUFamily5_v1

The GPU family 5, version 1 feature set for iOS.

### iOS GPU Family 4

case iOS_GPUFamily4_v2

The GPU family 4, version 2 feature set for iOS.

case iOS_GPUFamily4_v1

The GPU family 4, version 1 feature set for iOS.

### iOS GPU Family 3

case iOS_GPUFamily3_v4

The GPU family 3, version 4 feature set for iOS.

case iOS_GPUFamily3_v3

The GPU family 3, version 3 feature set for iOS.

case iOS_GPUFamily3_v2

The GPU family 3, version 2 feature set for iOS.

case iOS_GPUFamily3_v1

The GPU family 3, version 1 feature set for iOS.

### iOS GPU Family 2

case iOS_GPUFamily2_v5

The GPU family 2, version 5 feature set for iOS.

case iOS_GPUFamily2_v4

The GPU family 2, version 4 feature set for iOS.

case iOS_GPUFamily2_v3

The GPU family 2, version 3 feature set for iOS.

case iOS_GPUFamily2_v2

The GPU family 2, version 2 feature set for iOS.

case iOS_GPUFamily2_v1

The GPU family 2, version 1 feature set for iOS.

### iOS GPU Family 1

case iOS_GPUFamily1_v5

The GPU family 1, version 5 feature set for iOS.

case iOS_GPUFamily1_v4

The GPU family 1, version 4 feature set for iOS.

case iOS_GPUFamily1_v3

The GPU family 1, version 3 feature set for iOS.

case iOS_GPUFamily1_v2

The GPU family 1, version 2 feature set for iOS.

case iOS_GPUFamily1_v1

The GPU family 1, version 1 feature set for iOS.

### tvOS GPU Family 2

case tvOS_GPUFamily2_v2

The GPU family 2, version 2 feature set for tvOS.

case tvOS_GPUFamily2_v1

The GPU family 2, version 1 feature set for tvOS.

### tvOS GPU Family 1

case tvOS_GPUFamily1_v4

The GPU family 1, version 4 feature set for tvOS.

case tvOS_GPUFamily1_v3

The GPU family 1, version 3 feature set for tvOS.

case tvOS_GPUFamily1_v2

The GPU family 1, version 2 feature set for tvOS.

case tvOS_GPUFamily1_v1

The GPU family 1, version 1 feature set for tvOS.

### macOS GPU Family 2

case macOS_GPUFamily2_v1

The GPU family 2, version 1 feature set for macOS.

### macOS GPU Family 1

case macOS_GPUFamily1_v4

The GPU family 1, version 4 feature set for macOS.

case macOS_GPUFamily1_v3

The GPU family 1, version 3 feature set for macOS.

case macOS_GPUFamily1_v2

The GPU family 1, version 2 feature set for macOS.

case macOS_GPUFamily1_v1

The GPU family 1, version 1 feature set for macOS.

### macOS Tier 2

case macOS_ReadWriteTextureTier2

The read-write texture, tier 2 feature set for macOS.

### Initializers

init?(rawValue: UInt)

### Type Properties

static var osx_GPUFamily1_v1: MTLFeatureSet

static var osx_GPUFamily1_v2: MTLFeatureSet

static var osx_ReadWriteTextureTier2: MTLFeatureSet

static var tvos_GPUFamily1_v1: MTLFeatureSet

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

enum MTLGPUFamily

Represents the functionality for families of GPUs.

func supportsFeatureSet(MTLFeatureSet) -> Bool

Returns a Boolean value that indicates whether the GPU device supports a specific feature set.

**Required**

Deprecated

