

- Core Spotlight
-  CSSearchableItemActivityIdentifier 

Global Variable

# CSSearchableItemActivityIdentifier

The key you use to access a searchable item in a user activity object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
let CSSearchableItemActivityIdentifier: String
```

## Discussion

Use this key to access the unique identifier for the searchable item from the userInfo dictionary of a NSUserActivity object.

## See Also

### Continuing a search or activity

let CSSearchableItemActionType: String

Indicates that the activity type to continue is related to a searchable item.

let CSQueryContinuationActionType: String

Indicates that the activity type to continue is a search or query.

let CSSearchQueryString: String

Provides the key for the current query in the info dictionary of the user activity object.

