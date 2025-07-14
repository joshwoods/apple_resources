

- Metal
- MTLPipelineBufferDescriptorArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the pipeline buffer descriptor at the specified array index.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
subscript(bufferIndex: Int) -> MTLPipelineBufferDescriptor! { get set }
```

## Parameters 

`bufferIndex`  

The array index of the requested pipeline buffer descriptor.

## Return Value

The descriptor for the buffer bound at this index.

