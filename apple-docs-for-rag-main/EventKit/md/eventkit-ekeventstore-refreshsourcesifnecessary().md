

- EventKit
- EKEventStore
-  refreshSourcesIfNecessary() 

Instance Method

# refreshSourcesIfNecessary()

Pulls new data from remote sources, if necessary.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+

``` source
func refreshSourcesIfNecessary()
```

## Discussion

Use this method to pull new data from remote sources if the local data is out of date.

## See Also

### Saving and restoring state

func commit() throws

Commits all unsaved changes to the event store.

func reset()

Reverts the event store to its saved state.

