

- Core Media
-  CMBufferQueueInstallTriggerHandlerWithIntegerThreshold(\_:\_:\_:\_:\_:) 

Function

# CMBufferQueueInstallTriggerHandlerWithIntegerThreshold(\_:\_:\_:\_:\_:)

Installs a trigger with a handler and threshold on a buffer queue.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.14.4+tvOS 12.2+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueInstallTriggerHandlerWithIntegerThreshold(
    _ queue: CMBufferQueue,
    _ condition: CMBufferQueueTriggerCondition,
    _ threshold: CMItemCount,
    _ triggerTokenOut: UnsafeMutablePointer?,
    _ handler: CMBufferQueueTriggerHandler?
) -> OSStatus
```

## See Also

### Managing Triggers

func CMBufferQueueInstallTriggerHandler(CMBufferQueue, CMBufferQueueTriggerCondition, CMTime, UnsafeMutablePointer&lt;CMBufferQueueTriggerToken?>?, CMBufferQueueTriggerHandler?) -> OSStatus

Installs a trigger with a handler on a buffer queue.

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

func CMBufferQueueInstallTriggerWithIntegerThreshold(CMBufferQueue, callback: CMBufferQueueTriggerCallback?, refcon: UnsafeMutableRawPointer?, condition: CMBufferQueueTriggerCondition, threshold: CMItemCount, triggerTokenOut: UnsafeMutablePointer&lt;CMBufferQueueTriggerToken?>?) -> OSStatus

Installs a trigger with a callback and threshold on a buffer queue.

typealias CMBufferQueueTriggerCallback

A callback for the system to invoke when a trigger condition becomes true.

typealias CMBufferQueueTriggerCondition

A type to specify conditions to associate with a buffer queue trigger.

