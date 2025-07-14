

- Core Media
- CMBufferQueue
-  setValidationHandler(\_:) 

Instance Method

# setValidationHandler(\_:)

Sets validation handler for the queue to call before enqueuing buffers.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setValidationHandler(_ body: @escaping (CMBufferQueue, CMBuffer) throws -> Void)
```

