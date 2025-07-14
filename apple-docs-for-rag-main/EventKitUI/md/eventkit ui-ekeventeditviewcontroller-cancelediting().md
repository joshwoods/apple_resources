

- EventKit UI
- EKEventEditViewController
-  cancelEditing() 

Instance Method

# cancelEditing()

Ends the editing session and discards any changes that were made to the event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func cancelEditing()
```

## Discussion

This method is the programmatic equivalent of the user tapping Cancel. The delegate won’t receive the eventEditViewController(_:didCompleteWith:) message, so you must dismiss the controller after calling this method.

