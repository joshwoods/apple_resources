

- Foundation
- NSUserActivity
-  targetContentIdentifier 

Instance Property

# targetContentIdentifier

A string that identifies the user activity’s content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var targetContentIdentifier: String? { get set }
```

## Discussion

A target content identifier is a string you define within your app. This string provides a unique identifier for specific content in your app, like a particular document or the location of a piece of data in a database. This string isn’t visible to the user.

If you set this property, when the system delivers an NSUserActivity object to an app with multiple scenes, it chooses the UIScene whose UISceneActivationConditions have the best match with the target content identifier. For more information, see UISceneActivationConditions.

This property is optional but is highly recommended to create a great multitasking experience for apps that run on iPad. Setting this property doesn’t automatically set needsSave to true.

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

var needsSave: Bool

A Boolean value that indicates whether the state of the activity needs to be updated.

var contentAttributeSet: CSSearchableItemAttributeSet?

A set of properties that describe the activity.

var keywords: Set&lt;String>

A set of localized keywords that can help users find the activity in search results.

var persistentIdentifier: NSUserActivityPersistentIdentifier?

A value used to identify the user activity.

typealias NSUserActivityPersistentIdentifier

The type that defines a persistent identifier value for a user activity.

var appClipActivationPayload: APActivationPayload?

An object containing the payload information that launches an App Clip.

