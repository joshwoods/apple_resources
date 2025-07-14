

- HomeKit
- HMTrigger
-  uniqueIdentifier 

Instance Property

# uniqueIdentifier

A unique identifier for this trigger.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var uniqueIdentifier: UUID { get }
```

## See Also

### Managing Triggers

var name: String

The name of the trigger.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the trigger.

var isEnabled: Bool

State of the trigger.

func enable(Bool, completionHandler: ((any Error)?) -> Void)

Changes the enabled state of the trigger.

var lastFireDate: Date?

The last time this trigger fired.

Deprecated

