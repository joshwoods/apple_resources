

- HomeKit
- HMTrigger
-  enable(\_:completionHandler:) 

Instance Method

# enable(\_:completionHandler:)

Changes the enabled state of the trigger.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func enable(
    _ enable: Bool,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func enable(_ enable: Bool) async throws
```

## Parameters 

`enable`  

`TRUE` to enable the trigger, false to disable it.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

Triggers can only be enabled when they are in a home. You add triggers to a home using the addTrigger(_:completionHandler:) method of HMHome.

When a trigger is enabled its firing conditions are checked for validity and the system starts tracking the trigger and when it will next fire.

In addition to having valid firing conditions, to be successfully enabled a trigger must have at least one action set associated with it, and every action set associated with the trigger must have at least one action.

## See Also

### Managing Triggers

var name: String

The name of the trigger.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the trigger.

var isEnabled: Bool

State of the trigger.

var lastFireDate: Date?

The last time this trigger fired.

Deprecated

var uniqueIdentifier: UUID

A unique identifier for this trigger.

