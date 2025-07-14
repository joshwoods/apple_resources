

- Group Activities
- GroupSession
-  activity 

Instance Property

# activity

The current activity associated with the session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@Published
final var activity: ActivityType { get set }
```

## Discussion

Use this property to fetch information about the selected activity. The value in this property conforms to the GroupActivity protocol. Use it to fetch the activity details.

The participants of a session may change the current activity at any time, and the session updates this property dynamically to reflect any changes. Subscribe to the property to listen for changes, and update your app’s activity to match.

Important

Update this property only when the activity is in the GroupSession.State.joined state; otherwise, the behavior is undefined.

