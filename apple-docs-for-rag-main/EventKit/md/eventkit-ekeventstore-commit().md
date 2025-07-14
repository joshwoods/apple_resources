

- EventKit
- EKEventStore
-  commit() 

Instance Method

# commit()

Commits all unsaved changes to the event store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+

``` source
func commit() throws
```

## Mentioned in 

Creating events and reminders

## Discussion

This method allows you to save batched changes to the event store. For example, if you pass false as the `commit` parameter to the saveCalendar(_:commit:), removeCalendar(_:commit:), save(_:span:commit:), or remove(_:span:commit:) methods, the changes aren’t saved until commit() is invoked. Likewise, if you pass true as the `commit` parameter to the above methods, you don’t need to call commit().

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. Call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Saving and restoring state

func reset()

Reverts the event store to its saved state.

func refreshSourcesIfNecessary()

Pulls new data from remote sources, if necessary.

