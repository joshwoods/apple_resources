

- Metal
- MTLDevice
-  supportsFeatureSet(\_:) Deprecated

Instance Method

# supportsFeatureSet(\_:)

Returns a Boolean value that indicates whether the GPU device supports a specific feature set.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func supportsFeatureSet(_ featureSet: MTLFeatureSet) -> Bool
```

**Required**

Deprecated

Use the supportsFamily(_:) method instead if your app is running on an OS that supports that method.

## Parameters 

`featureSet`  

A MTLFeatureSet instance.

## See Also

### Related Documentation

Detecting GPU Features and Metal Software Versions

Use the device object’s properties to determine how you perform tasks in Metal.

### Checking a GPU Device’s Feature Support

func supportsFamily(MTLGPUFamily) -> Bool

Returns a Boolean value that indicates whether the GPU device supports the feature set of a specific GPU family.

**Required**

enum MTLGPUFamily

Represents the functionality for families of GPUs.

enum MTLFeatureSet

The device feature sets that define specific platform, hardware, and software configurations.

Deprecated

