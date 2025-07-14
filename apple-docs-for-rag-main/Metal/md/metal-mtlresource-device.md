

- Metal
- MTLResource
-  device 

Instance Property

# device

The device object that created the resource.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

A resource can only be used with the MTLDevice that created it.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Identifying the Resource

var label: String?

A string that identifies the resource.

**Required**

