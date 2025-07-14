

- ClassKit
- CLSActivity
-  removeAllActivityItems() 

Instance Method

# removeAllActivityItems()

Deletes all activity items associated with the current activity.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
func removeAllActivityItems()
```

## Discussion

Call the save(completion:) method on the data store after removing activity items, just as you would when adding items, to propagate the changes to the network:

```
activity.removeAllActivityItems()

CLSDataStore.shared.save { error in
    // Handle errors.
}
```

## See Also

### Managing activity items

func addAdditionalActivityItem(CLSActivityItem)

Adds an activity item to an activity.

var primaryActivityItem: CLSActivityItem?

Adds an activity item to an activity and sets it as the primary activity item.

var additionalActivityItems: [CLSActivityItem]

The list of activity items associated with an activity.

