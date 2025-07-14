

- Core Bluetooth
- CBCentralManager
-  supports(\_:) 

Type Method

# supports(\_:)

Returns a Boolean that indicates whether the device supports a specific set of features.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func supports(_ features: CBCentralManager.Feature) -> Bool
```

## Parameters 

`features`  

One or more features that you would like to check for support.

## See Also

### Inspecting Feature Support

struct Feature

An option set of device-specific features.

