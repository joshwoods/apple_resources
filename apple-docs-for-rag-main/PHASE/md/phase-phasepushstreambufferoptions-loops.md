

- PHASE
- PHASEPushStreamBufferOptions
-  loops 

Type Property

# loops

Indicates a buffer restarts after it finishes processing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var loops: PHASEPushStreamBufferOptions { get }
```

## See Also

### Options

static var `default`: PHASEPushStreamBufferOptions

Indicates a buffer processes after existing buffers in the queue.

static var interrupts: PHASEPushStreamBufferOptions

Indicates a buffer begins processing immediately.

static var interruptsAtLoop: PHASEPushStreamBufferOptions

Indicates a buffer begins processing when an existing buffer loops.

