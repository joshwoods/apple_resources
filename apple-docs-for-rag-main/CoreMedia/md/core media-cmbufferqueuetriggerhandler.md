

- Core Media
-  CMBufferQueueTriggerHandler 

Type Alias

# CMBufferQueueTriggerHandler

A type alias for a trigger handler.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.14.4+tvOS 12.2+visionOS 1.0+watchOS 6.0+

``` source
typealias CMBufferQueueTriggerHandler = (CMBufferQueueTriggerToken) -> Void
```

## See Also

### Managing Triggers

func CMBufferQueueInstallTriggerHandler(CMBufferQueue, CMBufferQueueTriggerCondition, CMTime, UnsafeMutablePointer&lt;CMBufferQueueTriggerToken?>?, CMBufferQueueTriggerHandler?) -> OSStatus

Installs a trigger with a handler on a buffer queue.

func CMBufferQueueInstallTriggerHandlerWithIntegerThreshold(CMBufferQueue, CMBufferQueueTriggerCondition, CMItemCount, UnsafeMutablePointer&lt;CMBufferQueueTriggerToken?>?, CMBufferQueueTriggerHandler?) -> OSStatus

Installs a trigger with a handler and threshold on a buffer queue.

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

