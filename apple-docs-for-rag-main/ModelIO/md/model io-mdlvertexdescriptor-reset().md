

- Model I/O
- MDLVertexDescriptor
-  reset() 

Instance Method

# reset()

Resets a vertex descriptor to its default state.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func reset()
```

## Discussion

Calling this method returns the descriptor to its original state, as is produced when initializing a vertex descriptor with the inherited init() method. After calling this method, the descriptor contains a single empty MDLVertexAttribute object and a single empty MDLVertexBufferLayout object.

