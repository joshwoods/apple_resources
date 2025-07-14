

- EventKit UI
- EKEventEditViewDelegate
-  eventEditViewController(\_:didCompleteWith:) 

Instance Method

# eventEditViewController(\_:didCompleteWith:)

Invoked when the user finishes editing an event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func eventEditViewController(
    _ controller: EKEventEditViewController,
    didCompleteWith action: EKEventEditViewAction
)
```

**Required**

## Parameters 

`controller`  

The edit view controller presenting the event.

`action`  

The action the user took to end editing.

## Discussion

Implement this method to dismiss the modal event edit view controller.

## See Also

### Finishing an Edit

enum EKEventEditViewAction

The action taken by the user after editing an event.

