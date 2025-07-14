

- Core Media
-  CMBufferQueueInstallTriggerWithIntegerThreshold(\_:callback:refcon:condition:threshold:triggerTokenOut:) 

Function

# CMBufferQueueInstallTriggerWithIntegerThreshold(\_:callback:refcon:condition:threshold:triggerTokenOut:)

Installs a trigger with a callback and threshold on a buffer queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueInstallTriggerWithIntegerThreshold(
    _ queue: CMBufferQueue,
    callback: CMBufferQueueTriggerCallback?,
    refcon: UnsafeMutableRawPointer?,
    condition: CMBufferQueueTriggerCondition,
    threshold: CMItemCount,
    triggerTokenOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`queue`  

`CMBufferQueue` on which the trigger is being set.

`callback`  

Callback to be called when the trigger condition becomes true. Can be `NULL`, if client intends only to explicitly test the condition. Cannot be `NULL` if triggerTokenOut is NULL, otherwise the trigger would be meaningless.

`refcon`  

Refcon to be passed to the triggerCallback. Can be `NULL` if the callback doesn’t need it, or is itself `NULL`.\`\`

`condition`  

The condition to be tested when evaluating the trigger. Must be a valid condition for an integer threshold.

`threshold`  

The integer value to compare against when evaluating the trigger.

`triggerTokenOut`  

Address where created trigger token will be written. Can be `NULL`, if client has no need to explicitly test or remove the trigger. Cannot be `NULL` if triggerCallback is NULL, since the trigger would be meaningless then.

## Return Value

A result code. See `Result Codes`

## Discussion

This function behaves the same way as CMBufferQueueInstallTrigger(_:callback:refcon:condition:time:triggerTokenOut:) except the trigger is evaluated against the integer value rather than the time value.

## See Also

### Managing Triggers

func CMBufferQueueInstallTriggerHandler(CMBufferQueue, CMBufferQueueTriggerCondition, CMTime, UnsafeMutablePointer&lt;CMBufferQueueTriggerToken?>?, CMBufferQueueTriggerHandler?) -> OSStatus

Installs a trigger with a handler on a buffer queue.

func CMBufferQueueInstallTriggerHandlerWithIntegerThreshold(CMBufferQueue, CMBufferQueueTriggerCondition, CMItemCount, UnsafeMutablePointer&lt;CMBufferQueueTriggerToken?>?, CMBufferQueueTriggerHandler?) -> OSStatus

Installs a trigger with a handler and threshold on a buffer queue.

typealias CMBufferQueueTriggerHandler

A type alias for a trigger handler.

typealias CMBufferQueueTriggerToken

A type alias for a trigger token.

Buffer Trigger Conditions

The trigger conditions the framework supports.

func CMBufferQueueTestTrigger(CMBufferQueue, triggerToken: CMBufferQueueTriggerToken) -> Bool

Tests whether the trigger condition is true for the specified buffer queue.

func CMBufferQueueInstallTrigger(CMBufferQueue, callback: CMBufferQueueTriggerCallback?, refcon: UnsafeMutableRawPointer?, condition: CMBufferQueueTriggerCondition, time: CMTime, triggerTokenOut: UnsafeMutablePointer&lt;CMBufferQueueTriggerToken?>?) -> OSStatus

Installs a trigger with a callback on a buffer queue.

typealias CMBufferQueueTriggerCallback

A callback for the system to invoke when a trigger condition becomes true.

typealias CMBufferQueueTriggerCondition

A type to specify conditions to associate with a buffer queue trigger.

