

- Core Media
- CMBufferQueue
-  CMBufferQueue.TriggerCondition 

Enumeration

# CMBufferQueue.TriggerCondition

An enumeration of trigger conditions.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum TriggerCondition
```

## Topics

### Conditions

case whenBufferCountBecomesGreaterThan(CMItemCount)

case whenBufferCountBecomesLessThan(CMItemCount)

case whenDataBecomesReady

case whenDurationBecomesGreaterThan(CMTime)

case whenDurationBecomesGreaterThanOrEqualTo(CMTime)

case whenDurationBecomesLessThan(CMTime)

case whenDurationBecomesLessThanOrEqualTo(CMTime)

case whenEndOfDataReached

case whenMaxPresentationTimeStampChanges

case whenMinPresentationTimeStampChanges

case whenReset

## Relationships

### Conforms To

- Sendable

## See Also

### Managing Triggers

func installTrigger(condition: CMBufferQueue.TriggerCondition, CMBufferQueueTriggerHandler?) throws -> CMBufferQueue.TriggerToken

Installs a trigger on the queue.

func removeTrigger(CMBufferQueue.TriggerToken) throws

Removes a trigger from the queue.

func testTrigger(CMBufferQueue.TriggerToken) -> Bool

Tests a trigger condition.

typealias TriggerToken

A type alias for a trigger token.

