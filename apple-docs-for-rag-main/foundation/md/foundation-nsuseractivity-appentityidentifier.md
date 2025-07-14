

- Foundation
- NSUserActivity
-  appEntityIdentifier 

Instance Property

# appEntityIdentifier

The identifier of an app entity that you associate with the user activity.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
var appEntityIdentifier: EntityIdentifier? { get set }
```

## Discussion

By associating an app entity with a user activity, you make the entity available to Siri and Apple Intelligence. To clear the association with the app entity, set `appEntityIdentifier` to `nil`.

For more information, refer to Making onscreen content available to Siri and Apple Intelligence and App Intents.

