

- PHASE
- PHASEPushStreamBufferOptions
-  interruptsAtLoop 

Type Property

# interruptsAtLoop

Indicates a buffer begins processing when an existing buffer loops.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var interruptsAtLoop: PHASEPushStreamBufferOptions { get }
```

## See Also

### Options

static var `default`: PHASEPushStreamBufferOptions

Indicates a buffer processes after existing buffers in the queue.

static var interrupts: PHASEPushStreamBufferOptions

Indicates a buffer begins processing immediately.

static var loops: PHASEPushStreamBufferOptions

Indicates a buffer restarts after it finishes processing.

