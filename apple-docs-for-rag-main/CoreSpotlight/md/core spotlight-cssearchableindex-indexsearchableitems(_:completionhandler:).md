

- Core Spotlight
- CSSearchableIndex
-  indexSearchableItems(\_:completionHandler:) 

Instance Method

# indexSearchableItems(\_:completionHandler:)

Adds or updates items in the index.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func indexSearchableItems(
    _ items: [CSSearchableItem],
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func indexSearchableItems(_ items: [CSSearchableItem]) async throws
```

## Parameters 

`items`  

An array of searchable items to add or update.

`completionHandler`  

The block that’s called when the data has been journaled by the index, which means that the index makes a note that it has to perform this operation. If the completion handler returns an error, it means that the data wasn’t journaled correctly and the client should retry the request.

The block receives the following parameter:

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Mentioned in 

Adding your app’s content to Spotlight indexes

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func indexSearchableItems(_ items: [CSSearchableItem]) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The searchableIndex(_:reindexSearchableItemsWithIdentifiers:acknowledgementHandler:) protocol method is called in the case that the journaling completed successfully but the data was not able to be indexed for some reason.

## See Also

### Managing items in an index

func deleteAllSearchableItems(completionHandler: (((any Error)?) -> Void)?)

Deletes all searchable items from the index.

func deleteSearchableItems(withDomainIdentifiers: [String], completionHandler: (((any Error)?) -> Void)?)

Removes from the index all searchable items associated with the specified domain.

func deleteSearchableItems(withIdentifiers: [String], completionHandler: (((any Error)?) -> Void)?)

Removes from the index all items with the specified identifiers.

