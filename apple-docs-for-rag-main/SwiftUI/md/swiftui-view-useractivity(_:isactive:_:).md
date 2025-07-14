

- SwiftUI
- View
-  userActivity(\_:isActive:\_:) 

Instance Method

# userActivity(\_:isActive:\_:)

Advertises a user activity type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func userActivity(
    _ activityType: String,
    isActive: Bool = true,
    _ update: @escaping (NSUserActivity) -> ()
) -> some View
```

## Parameters 

`activityType`  

The type of activity to advertise.

`isActive`  

When `false`, avoids advertising the activity. Defaults to `true`.

`update`  

A function that modifies the passed-in activity for advertisement.

## Discussion

You can use `userActivity(_:isActive:_:)` to start, stop, or modify the advertisement of a specific type of user activity.

The scope of the activity applies only to the scene or window the view is in.

## See Also

### Sending and receiving user activities

Restoring Your App’s State with SwiftUI

Provide app continuity for users by preserving their current activities.

func userActivity&lt;P>(String, element: P?, (P, NSUserActivity) -> ()) -> some View

Advertises a user activity type.

func onContinueUserActivity(String, perform: (NSUserActivity) -> ()) -> some View

Registers a handler to invoke in response to a user activity that your app receives.

