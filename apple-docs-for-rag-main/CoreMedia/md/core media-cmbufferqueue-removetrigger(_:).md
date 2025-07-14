

- Core Media
- CMBufferQueue
-  removeTrigger(\_:) 

Instance Method

# removeTrigger(\_:)

Removes a trigger from the queue.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func removeTrigger(_ triggerToken: CMBufferQueue.TriggerToken) throws
```

## See Also

### Managing Triggers

func installTrigger(condition: CMBufferQueue.TriggerCondition, CMBufferQueueTriggerHandler?) throws -> CMBufferQueue.TriggerToken

Installs a trigger on the queue.

func testTrigger(CMBufferQueue.TriggerToken) -> Bool

Tests a trigger condition.

typealias TriggerToken

A type alias for a trigger token.

enum TriggerCondition

An enumeration of trigger conditions.

