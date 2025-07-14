

- DeviceActivity
- DeviceActivityReport
-  userActivity(\_:isActive:\_:) 

Instance Method

# userActivity(\_:isActive:\_:)

Advertises a user activity type.

DeviceActivitySwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

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

