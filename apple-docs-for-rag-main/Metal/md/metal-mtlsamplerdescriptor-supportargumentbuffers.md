

- Metal
- MTLSamplerDescriptor
-  supportArgumentBuffers 

Instance Property

# supportArgumentBuffers

A Boolean value that indicates whether you can reference a sampler, that you make with this descriptor, by its resource ID from an argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var supportArgumentBuffers: Bool { get set }
```

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

## Discussion

The default value is false, which means that you can only encode the samplers you make with this descriptor as individual resources in the sampler state argument table.

Your app can encode samplers into an argument buffer if you create them with an MTLSamplerDescriptor instance that has this property equal to true.

Tip

Check maxArgumentBufferSamplerCount at runtime to query the number of samplers your app can encode into an argument buffer.

Each unique configuration of an MTLSamplerDescriptor instance’s properties creates a unique MTLSamplerState instance. For example, you can create unique samplers with the same MTLSamplerDescriptor instance by changing one or more values of its properties, such as minFilter or magFilter before creating another instance.

Conversely, creating secondary sampler instances with the same descriptor property values doesn’t create any additional, unique samplers. Instead, they refer to the same underlying sampler, even if you create it with a difference descriptor instance because the configuration is the same.

