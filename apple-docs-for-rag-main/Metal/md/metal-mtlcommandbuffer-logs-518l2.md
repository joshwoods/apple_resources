

- Metal
- MTLCommandBuffer
-  logs 

Instance Property

# logs

The messages the command buffer records as the GPU runs its commands.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOS

``` source
var logs: MTLLogContainer { get }
```

## Discussion

The value of this property is valid only after the command buffer finishes executing.

