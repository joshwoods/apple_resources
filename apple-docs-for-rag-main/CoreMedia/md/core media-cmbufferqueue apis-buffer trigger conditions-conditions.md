

- Core Media
- CMBufferQueue APIs
-  Buffer Trigger Conditions 

API Collection

# Buffer Trigger Conditions

The trigger conditions the framework supports.

## Topics

### Constants

var kCMBufferQueueTrigger_WhenDurationBecomesLessThan: CMBufferQueueTriggerCondition

Trigger fires when queue duration becomes less than the specified duration.

var kCMBufferQueueTrigger_WhenDurationBecomesLessThanOrEqualTo: CMBufferQueueTriggerCondition

Trigger fires when queue duration becomes less than or equal to the specified duration.

var kCMBufferQueueTrigger_WhenDurationBecomesGreaterThan: CMBufferQueueTriggerCondition

Trigger fires when queue duration becomes greater than the specified duration.

var kCMBufferQueueTrigger_WhenDurationBecomesGreaterThanOrEqualTo: CMBufferQueueTriggerCondition

Trigger fires when queue duration becomes greater than or equal to the specified duration.

var kCMBufferQueueTrigger_WhenMinPresentationTimeStampChanges: CMBufferQueueTriggerCondition

Trigger fires when the minimum presentation timestamp changes (triggerDuration is ignored).

var kCMBufferQueueTrigger_WhenMaxPresentationTimeStampChanges: CMBufferQueueTriggerCondition

Trigger fires when the maximum presentation timestamp changes (triggerDuration is ignored).

var kCMBufferQueueTrigger_WhenDataBecomesReady: CMBufferQueueTriggerCondition

Trigger fires when next dequeueable buffer becomes ready (that is, CMBufferQueueDequeueIfDataReady(_:) will now succeed). (triggerDuration is ignored.)

var kCMBufferQueueTrigger_WhenEndOfDataReached: CMBufferQueueTriggerCondition

Trigger fires when CMBufferQueueIsAtEndOfData’s condition becomes true. (triggerDuration is ignored.)

var kCMBufferQueueTrigger_WhenReset: CMBufferQueueTriggerCondition

Trigger fires when CMBufferQueueReset called. (triggerDuration is ignored.)

var kCMBufferQueueTrigger_WhenBufferCountBecomesLessThan: CMBufferQueueTriggerCondition

Trigger fires when buffer count becomes less than the specified threshold number.

var kCMBufferQueueTrigger_WhenBufferCountBecomesGreaterThan: CMBufferQueueTriggerCondition

Trigger fires when buffer count becomes \> the specified threshold number.

var kCMBufferQueueTrigger_WhenDurationBecomesGreaterThanOrEqualToAndBufferCountBecomesGreaterThan: CMBufferQueueTriggerCondition

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

