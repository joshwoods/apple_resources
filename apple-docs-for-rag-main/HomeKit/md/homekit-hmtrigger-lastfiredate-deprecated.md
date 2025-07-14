

- HomeKit
- HMTrigger
-  lastFireDate Deprecated

Instance Property

# lastFireDate

The last time this trigger fired.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–10.0Deprecated

``` source
var lastFireDate: Date? { get }
```

Deprecated

This property is no longer supported.

## Discussion

`nil` if the trigger has never fired.

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

var uniqueIdentifier: UUID

A unique identifier for this trigger.

