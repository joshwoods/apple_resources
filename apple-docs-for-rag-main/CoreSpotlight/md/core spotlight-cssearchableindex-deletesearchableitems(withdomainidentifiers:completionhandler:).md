

- Core Spotlight
- CSSearchableIndex
-  deleteSearchableItems(withDomainIdentifiers:completionHandler:) 

Instance Method

# deleteSearchableItems(withDomainIdentifiers:completionHandler:)

Removes from the index all searchable items associated with the specified domain.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func deleteSearchableItems(
    withDomainIdentifiers domainIdentifiers: [String],
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func deleteSearchableItems(withDomainIdentifiers domainIdentifiers: [String]) async throws
```

## Parameters 

`domainIdentifiers`  

The domain identifier that describes the group of items to delete. To learn more about domain identifiers, see domainIdentifier.

`completionHandler`  

The block that’s called when the request has been journaled by the index (“journaled” means that the index makes a note that it has to perform this operation). Note that the request may not have completed.

The block receives the following parameter:

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func deleteSearchableItems(withDomainIdentifiers domainIdentifiers: [String]) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to delete groups of items. Note that the delete operation is recursive. For example, if domain identifiers are of the form `.`, calling this method and specifying `` deletes items with the specified account and any mailbox.

## See Also

### Managing items in an index

func indexSearchableItems([CSSearchableItem], completionHandler: (((any Error)?) -> Void)?)

Adds or updates items in the index.

func deleteAllSearchableItems(completionHandler: (((any Error)?) -> Void)?)

Deletes all searchable items from the index.

func deleteSearchableItems(withIdentifiers: [String], completionHandler: (((any Error)?) -> Void)?)

Removes from the index all items with the specified identifiers.

