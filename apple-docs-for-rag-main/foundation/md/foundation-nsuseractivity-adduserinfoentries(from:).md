

- Foundation
- NSUserActivity
-  addUserInfoEntries(from:) 

Instance Method

# addUserInfoEntries(from:)

Adds the contents of the specified dictionary to the user info dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addUserInfoEntries(from otherDictionary: [AnyHashable : Any])
```

## Parameters 

`otherDictionary`  

The dictionary containing entries to be added.

## Mentioned in 

Implementing Handoff in Your App

## Discussion

Use this method to add the keys from `otherDictionary` into the dictionary in the userInfo property. If the same key is in both dictionaries, the value of the key is set to the value in the `otherDictionary` parameter.

It’s recommended that you keep the userInfo dictionary as small as possible. The larger the dictionary, the longer it takes to deliver that payload and resume the activity.

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

var targetContentIdentifier: String?

A string that identifies the user activity’s content.

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

