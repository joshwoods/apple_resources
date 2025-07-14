

- HomeKit
- HMTrigger
-  name 

Instance Property

# name

The name of the trigger.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String { get }
```

## Discussion

Trigger names should be set by the user.

## See Also

### Related Documentation

HomeKit Developer Guide

### Managing Triggers

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the trigger.

var isEnabled: Bool

State of the trigger.

func enable(Bool, completionHandler: ((any Error)?) -> Void)

Changes the enabled state of the trigger.

var lastFireDate: Date?

The last time this trigger fired.

Deprecated

var uniqueIdentifier: UUID

A unique identifier for this trigger.

