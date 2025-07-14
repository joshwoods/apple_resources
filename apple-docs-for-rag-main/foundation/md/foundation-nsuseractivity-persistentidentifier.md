

- Foundation
- NSUserActivity
-  persistentIdentifier 

Instance Property

# persistentIdentifier

A value used to identify the user activity.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 5.0+

``` source
var persistentIdentifier: NSUserActivityPersistentIdentifier? { get set }
```

## Discussion

Set this property to a value that identifies the user activity so you can later delete it with deleteSavedUserActivities(withPersistentIdentifiers:completionHandler:). For example, if the user checks the weather for Cupertino each morning from home, the weather app sets the persistent identifier to the city name (Cupertino). When the user deletes Cupertino from the weather app, the app deletes the user activity associated with the identifier, “Cupertino”.

```
let userActivity = NSUserActivity(activityType: WeatherLookup.userActivityType)
userActivity.persistentIdentifier = "Cupertino"
```

## See Also

### Accessing activity information

var activityType: String

The user activity object’s activity type.

var title: String?

An optional, user-visible title for this activity, such as a document name or web page title.

var requiredUserInfoKeys: Set&lt;String>?

A set of keys that represent the minimal information about the activity that should be stored for later restoration.

var userInfo: [AnyHashable : Any]?

A dictionary containing app-specific state information needed to continue an activity on another device.

func addUserInfoEntries(from: [AnyHashable : Any])

Adds the contents of the specified dictionary to the user info dictionary.

var targetContentIdentifier: String?

A string that identifies the user activity’s content.

var needsSave: Bool

A Boolean value that indicates whether the state of the activity needs to be updated.

var contentAttributeSet: CSSearchableItemAttributeSet?

A set of properties that describe the activity.

var keywords: Set&lt;String>

A set of localized keywords that can help users find the activity in search results.

typealias NSUserActivityPersistentIdentifier

The type that defines a persistent identifier value for a user activity.

var appClipActivationPayload: APActivationPayload?

An object containing the payload information that launches an App Clip.

