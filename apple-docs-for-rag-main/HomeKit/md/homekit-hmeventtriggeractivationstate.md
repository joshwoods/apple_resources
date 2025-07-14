

- HomeKit
-  HMEventTriggerActivationState 

Enumeration

# HMEventTriggerActivationState

The activation state of an event trigger.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum HMEventTriggerActivationState
```

## Topics

### Inspecting activation state

case disabled

Trigger is not activated.

case disabledNoCompatibleHomeHub

Trigger is not active because there is no compatible home hub.

case disabledNoHomeHub

Trigger is not active because there is no home hub.

case disabledNoLocationServicesAuthorization

Trigger is not active because the user has not authorized use of location services.

case enabled

The trigger is currently active.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Querying trigger activation state

var triggerActivationState: HMEventTriggerActivationState

The current activation state of the trigger.

