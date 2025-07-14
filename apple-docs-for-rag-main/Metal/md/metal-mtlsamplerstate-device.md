

- Metal
- MTLSamplerState
-  device 

Instance Property

# device

The device object that created the sampler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

A sampler is always associated with the MTLDevice that created it and can be used only with that device.

## See Also

### Identifying the Sampler

var label: String?

A string that identifies the sampler.

**Required**

