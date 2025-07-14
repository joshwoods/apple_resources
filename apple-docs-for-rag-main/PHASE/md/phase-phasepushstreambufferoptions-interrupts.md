

- PHASE
- PHASEPushStreamBufferOptions
-  interrupts 

Type Property

# interrupts

Indicates a buffer begins processing immediately.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var interrupts: PHASEPushStreamBufferOptions { get }
```

## See Also

### Options

static var `default`: PHASEPushStreamBufferOptions

Indicates a buffer processes after existing buffers in the queue.

static var interruptsAtLoop: PHASEPushStreamBufferOptions

Indicates a buffer begins processing when an existing buffer loops.

static var loops: PHASEPushStreamBufferOptions

Indicates a buffer restarts after it finishes processing.

