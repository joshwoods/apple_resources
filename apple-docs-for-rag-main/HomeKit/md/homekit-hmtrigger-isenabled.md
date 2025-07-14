

- HomeKit
- HMTrigger
-  isEnabled 

Instance Property

# isEnabled

State of the trigger.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var isEnabled: Bool { get }
```

## Discussion

Triggers that are not enabled never fire.

## See Also

### Managing Triggers

var name: String

The name of the trigger.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the trigger.

func enable(Bool, completionHandler: ((any Error)?) -> Void)

Changes the enabled state of the trigger.

var lastFireDate: Date?

The last time this trigger fired.

Deprecated

var uniqueIdentifier: UUID

A unique identifier for this trigger.

