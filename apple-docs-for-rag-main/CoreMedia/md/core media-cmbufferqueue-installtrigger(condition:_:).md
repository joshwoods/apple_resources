

- Core Media
- CMBufferQueue
-  installTrigger(condition:\_:) 

Instance Method

# installTrigger(condition:\_:)

Installs a trigger on the queue.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func installTrigger(
    condition: CMBufferQueue.TriggerCondition,
    _ body: CMBufferQueueTriggerHandler? = nil
) throws -> CMBufferQueue.TriggerToken
```

## See Also

### Managing Triggers

func removeTrigger(CMBufferQueue.TriggerToken) throws

Removes a trigger from the queue.

func testTrigger(CMBufferQueue.TriggerToken) -> Bool

Tests a trigger condition.

typealias TriggerToken

A type alias for a trigger token.

enum TriggerCondition

An enumeration of trigger conditions.

