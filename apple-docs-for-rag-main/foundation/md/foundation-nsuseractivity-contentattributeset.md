

- Foundation
- NSUserActivity
-  contentAttributeSet 

Instance Property

# contentAttributeSet

A set of properties that describe the activity.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@NSCopying
var contentAttributeSet: CSSearchableItemAttributeSet? { get set }
```

## Mentioned in 

Creating a user activity object

## Discussion

A CSSearchableItemAttributeSet object encapsulates the set of properties you want to display for a searchable activity.

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

var keywords: Set&lt;String>

A set of localized keywords that can help users find the activity in search results.

var persistentIdentifier: NSUserActivityPersistentIdentifier?

A value used to identify the user activity.

typealias NSUserActivityPersistentIdentifier

The type that defines a persistent identifier value for a user activity.

var appClipActivationPayload: APActivationPayload?

An object containing the payload information that launches an App Clip.

