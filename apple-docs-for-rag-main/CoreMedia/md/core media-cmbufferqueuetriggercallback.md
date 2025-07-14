

- Core Media
-  CMBufferQueueTriggerCallback 

Type Alias

# CMBufferQueueTriggerCallback

A callback for the system to invoke when a trigger condition becomes true.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMBufferQueueTriggerCallback = (UnsafeMutableRawPointer?, CMBufferQueueTriggerToken) -> Void
```

### Callback Parameters

triggerRefcon  
The contextual data.

triggerToken  
The trigger whose condition became true.

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

func CMBufferQueueInstallTriggerWithIntegerThreshold(CMBufferQueue, callback: CMBufferQueueTriggerCallback?, refcon: UnsafeMutableRawPointer?, condition: CMBufferQueueTriggerCondition, threshold: CMItemCount, triggerTokenOut: UnsafeMutablePointer&lt;CMBufferQueueTriggerToken?>?) -> OSStatus

Installs a trigger with a callback and threshold on a buffer queue.

typealias CMBufferQueueTriggerCondition

A type to specify conditions to associate with a buffer queue trigger.

