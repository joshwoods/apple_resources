

- ClassKit
- CLSDataStore
-  remove(\_:) 

Instance Method

# remove(\_:)

Marks a context for removal.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func remove(_ context: CLSContext)
```

## Parameters 

`context`  

The context to remove.

## Discussion

If your context hierarchy changes, either because your app’s content is dynamic, or as a result of an app update, you might need to remove old contexts from the data store. Call this method to mark a context for removal. Call the save(completion:) method to commit the change.

When you remove a context, the framework removes all of its decendants as well.

