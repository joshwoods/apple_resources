

- Metal
- MTLIndirectCommandBufferDescriptor
-  commandTypes 

Instance Property

# commandTypes

The set of command types that you can encode into the indirect command buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var commandTypes: MTLIndirectCommandType { get set }
```

## Discussion

When you create the indirect command buffer, Metal allocates memory for each command it can hold. It must allocate enough memory to hold any command that you might later encode. To save space, specify only the command types you are going to encode in the indirect command buffer.

You can’t combine rendering and compute commands in the same indirect command buffer.

