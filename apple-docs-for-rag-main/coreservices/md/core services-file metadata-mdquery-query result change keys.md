

- Core Services
- File Metadata
- MDQuery
-  Query Result Change Keys 

API Collection

# Query Result Change Keys

Specify the items that have changed in the query results.

## Topics

### Constants

let kMDQueryUpdateAddedItems: CFString!

An array that identifies the items that have been added to the query results. This list only contains result objects that have previously been created, result objects that have not been created are not included.

let kMDQueryUpdateChangedItems: CFString!

An array that identifies the items that have changed in the query results. This list only contains result objects that have previously been created, result objects that have not been created are not included.

let kMDQueryUpdateRemovedItems: CFString!

An array that identifies the items that have been removed from the query results. This list only contains result objects that have previously been created, result objects that have not been created are not included.

## See Also

### Notification Info Keys

Query Search Scope Keys

Specify the scope of a query’s search.

Result Relevance Sorting Key

Key used in a user notification’s description dictionary that indicates the relevance of a result.

