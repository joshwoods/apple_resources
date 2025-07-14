

- Core Media
- CMBufferQueue
-  CMBufferQueue.TriggerToken 

Type Alias

# CMBufferQueue.TriggerToken

A type alias for a trigger token.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias TriggerToken = CMBufferQueueTriggerToken
```

## See Also

### Managing Triggers

func installTrigger(condition: CMBufferQueue.TriggerCondition, CMBufferQueueTriggerHandler?) throws -> CMBufferQueue.TriggerToken

Installs a trigger on the queue.

func removeTrigger(CMBufferQueue.TriggerToken) throws

Removes a trigger from the queue.

func testTrigger(CMBufferQueue.TriggerToken) -> Bool

Tests a trigger condition.

enum TriggerCondition

An enumeration of trigger conditions.

