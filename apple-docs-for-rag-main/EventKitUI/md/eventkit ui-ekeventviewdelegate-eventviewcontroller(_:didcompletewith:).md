

- EventKit UI
- EKEventViewDelegate
-  eventViewController(\_:didCompleteWith:) 

Instance Method

# eventViewController(\_:didCompleteWith:)

Invoked when closing the event view controller.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
func eventViewController(
    _ controller: EKEventViewController,
    didCompleteWith action: EKEventViewAction
)
```

**Required**

## Parameters 

`controller`  

The event view controller to close.

`action`  

The action taken to prompt closing the event view controller. See EKEventViewAction for a list of possible values.

## See Also

### Responding to the Interface’s Dismissal

enum EKEventViewAction

Describes the action taken to close the event view controller.

