

- Core Spotlight
-  CSSearchableItemActionType 

Global Variable

# CSSearchableItemActionType

Indicates that the activity type to continue is related to a searchable item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
let CSSearchableItemActionType: String
```

## Discussion

The `CSSearchableItemActionType` and `CSSearchableItemActivityIdentifier` constants help your app restore state or an activity when a user opens a searchable item listed in a search result. When the user opens the item, Handoff calls your app delegate’s `application(_:willContinueUserActivityWithType:)` method with `CSSearchableItemActionType`. Handoff also delivers an `NSUserActivity` object that contains a `userInfo` dictionary in which the key is `CSSearchableItemActivityIdentifier` and the associated value is the unique identifier that was used when the item was created. Your app delegate can check for the unique identifier in its `application(_:continue:restorationHandler:)` method.

To learn more about enabling Handoff in your app, see the Handoff Programming Guide.

## See Also

### Continuing a search or activity

let CSSearchableItemActivityIdentifier: String

The key you use to access a searchable item in a user activity object.

let CSQueryContinuationActionType: String

Indicates that the activity type to continue is a search or query.

let CSSearchQueryString: String

Provides the key for the current query in the info dictionary of the user activity object.

