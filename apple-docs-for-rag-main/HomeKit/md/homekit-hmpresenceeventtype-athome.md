

- HomeKit
- HMPresenceEventType
-  atHome 

Type Property

# atHome

Triggers the event when at least one user is in the home.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
static var atHome: HMPresenceEventType { get }
```

## Discussion

A convenience value for use in predicates on HMEventTrigger. Represents the presence of at least one user in the home.

## See Also

### Using presence as a predicate

static var notAtHome: HMPresenceEventType

Triggers the event when there are no users in the home.

