

- Game Controller
- GCDevice
-  vendorName 

Instance Property

# vendorName

The manufacturer-provided name for the device, or the user’s name for the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var vendorName: String? { get }
```

**Required**

## Discussion

The value of this property may be `nil` and may not be unique. Use this property to present information about the device to the user.

## See Also

### Getting device information

var productCategory: String

The product category that identifies the type of controller.

**Required**

Product category constants

