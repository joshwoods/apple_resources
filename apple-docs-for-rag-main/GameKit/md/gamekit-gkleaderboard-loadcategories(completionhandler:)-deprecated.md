

- GameKit
- GKLeaderboard
-  loadCategories(completionHandler:) Deprecated

Type Method

# loadCategories(completionHandler:)

Loads the list of leaderboard categories along with their corresponding localized titles.

visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**visionOS, watchOS**

``` source
class func loadCategories(completionHandler: (([String]?, [String]?, (any Error)?) -> Void)? = nil)
```

**visionOS**

``` source
class func loadCategories() async throws -> ([String], [String])
```

Deprecated

Use the loadLeaderboards(completionHandler:) method instead.

## Parameters 

`completionHandler`  

A block to call after retrieving the categories from the server.

The block receives the following parameters:

*categories*  
An array of `NSString` objects that provides the categories to your game. If an error occurs, this value may be non-`nil`. In this case, the array holds whatever data GameKit downloads before the error occurs.

*titles*  
An array of `NSString` objects that provides localized titles for each category. If an error occurs, this value may be non-`nil`. In this case, the array holds whatever data GameKit downloads before the error occurs.

*error*  
If an error occurs, this error object describes the error. If the operation completes successfully, the value is `nil`.

## Discussion

You use this class method to retrieve the category identifiers and titles you configure for your leaderboards in App Store Connect. To create a leaderboard query that targets a particular category, set the category property to one of the strings that this method returns.

When you call this method, it creates a new background task to handle the request. The method then returns control to your game. When the task is complete, GameKit calls your completion handler on the main thread.

## See Also

### Deprecated methods

class func setDefault(String?, withCompletionHandler: (((any Error)?) -> Void)?)

Sets the default leaderboard for the local player.

Deprecated

class func loadLeaderboards(completionHandler: (([GKLeaderboard]?, (any Error)?) -> Void)?)

Loads a list of leaderboards from Game Center.

Deprecated

func loadScores(completionHandler: (([GKScore]?, (any Error)?) -> Void)?)

Retrieves a set of scores from Game Center.

Deprecated

