

- EventKit
- EKEvent
-  refresh() 

Instance Method

# refresh()

Updates the event’s data with the current information in the Calendar database.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func refresh() -> Bool
```

## Return Value

If the event was successfully refreshed, true; otherwise, false.

## Discussion

You should call this method only on events that your application is editing, and only when your application receives the EKEventStoreChangedNotification notification. If this method returns false, the event has been deleted or otherwise invalidated, and you should not continue to use it.

This method does not replace the values of any properties that you have modified.

