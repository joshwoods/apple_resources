

- Core Media
- CMBufferQueue
-  testTrigger(\_:) 

Instance Method

# testTrigger(\_:)

Tests a trigger condition.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func testTrigger(_ triggerToken: CMBufferQueue.TriggerToken) -> Bool
```

## See Also

### Managing Triggers

func installTrigger(condition: CMBufferQueue.TriggerCondition, CMBufferQueueTriggerHandler?) throws -> CMBufferQueue.TriggerToken

Installs a trigger on the queue.

func removeTrigger(CMBufferQueue.TriggerToken) throws

Removes a trigger from the queue.

typealias TriggerToken

A type alias for a trigger token.

enum TriggerCondition

An enumeration of trigger conditions.

