

- Metal
- MTLDevice
-  makeCommandQueue(descriptor:) 

Instance Method

# makeCommandQueue(descriptor:)

Creates a command queue with the provided configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func makeCommandQueue(descriptor: MTLCommandQueueDescriptor) -> (any MTLCommandQueue)?
```

**Required**

## Parameters 

`descriptor`  

The configuration for the new command queue.

