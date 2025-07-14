

- EventKit
- EKEventStore
-  reset() 

Instance Method

# reset()

Reverts the event store to its saved state.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func reset()
```

## Discussion

This method updates all the properties of all the objects with their corresponding values in the event store. Any local changes that aren’t saved before invoking this method are lost. All existing objects created or retrieved using this store are disassociated from it and are invalid.

## See Also

### Saving and restoring state

func commit() throws

Commits all unsaved changes to the event store.

func refreshSourcesIfNecessary()

Pulls new data from remote sources, if necessary.

