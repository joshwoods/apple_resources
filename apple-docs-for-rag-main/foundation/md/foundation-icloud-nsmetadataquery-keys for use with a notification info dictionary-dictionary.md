

- Foundation
- iCloud
- NSMetadataQuery
-  Keys for Use with a Notification Info Dictionary 

API Collection

# Keys for Use with a Notification Info Dictionary

Constants for keys to retrieve the collection of changed items from a notification’s user info dictionary.

## Overview

When querying the ubiquitous scope, these keys get added to the user info dictionary only in OS X v10.10 and iOS 8.0 or later, and only when iCloud Drive is enabled for the user’s iCloud account. To track changes in earlier versions of the SDK, use KVO on the query’s `results` property instead.

## Topics

### Constants

let NSMetadataQueryUpdateAddedItemsKey: String

The key for retrieving an array of items added to the query result. By default, this array contains NSMetadataItem objects, representing the query’s results; however, the query’s delegate can substitute these objects with instances of a different class.

let NSMetadataQueryUpdateChangedItemsKey: String

The key for retrieving an array of items that have changed in the query result. By default, this array contains NSMetadataItem objects, representing the query’s results; however, the query’s delegate can substitute these objects with instances of a different class.

let NSMetadataQueryUpdateRemovedItemsKey: String

The key for retrieving an array of items removed from the query result. By default, this array contains NSMetadataItem objects, representing the query’s results; however, the query’s delegate can substitute these objects with instances of a different class.

## See Also

### Constants

Metadata Query Search Scopes

Constants for the predefined search scopes used by searchScopes.

Content Relevance

In addition to including the requested metadata attributes, a query result also includes content relevance, accessed with the following key.

