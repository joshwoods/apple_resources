

- AppKit
- NSObjectController
-  fetch(with:merge:) 

Instance Method

# fetch(with:merge:)

Subclasses should override this method to customize a fetch request, for example to specify fetch limits.

macOS

``` source
func fetch(
    with fetchRequest: NSFetchRequest?,
    merge: Bool
) throws
```

## Parameters 

`fetchRequest`  

The fetch request to use for the fetch. Pass `nil` to use the default fetch request.

`merge`  

If true, the receiver merges the existing content with the fetch result, otherwise the receiver replaces the entire content with the fetch result.

## Discussion

This method performs a number of actions that you cannot reproduce. To customize this method, you should therefore create your own fetch request and then invoke `super`’s implementation with the new fetch request.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Core Data support

var entityName: String?

The entity name used by the receiver to create new objects.

func fetch(Any?)

Causes the receiver to fetch the data objects specified by the entity name and fetch predicate.

var usesLazyFetching: Bool

A Boolean that indicates whether the receiver uses lazy fetching.

func defaultFetchRequest() -> NSFetchRequest&lt;any NSFetchRequestResult>

Returns the default fetch request used by the receiver.

var fetchPredicate: NSPredicate?

The receiver’s fetch predicate.

var managedObjectContext: NSManagedObjectContext?

The receiver’s managed object context.

