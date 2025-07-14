

- ActivityKit
- Activity
-  end(\_:dismissalPolicy:timestamp:) 

Instance Method

# end(\_:dismissalPolicy:timestamp:)

Ends an active Live Activity.

iOS 17.2+iPadOS 17.2+

``` source
func end(
    _ content: ActivityContent.ContentState>?,
    dismissalPolicy: ActivityUIDismissalPolicy = .default,
    timestamp: Date
) async
```

## Parameters 

`content`  

The latest and final dynamic content for the Live Activity that ended. The size of the encoded content can’t exceed 4KB in size.

`dismissalPolicy`  

Describes how and when the system should dismiss a Live Activity and and remove it from the Lock Screen.

`timestamp`  

The time the data in the payload was generated. If this is older than a previous update or push payload, the system ignores this update.

## Discussion

End an active Live Activity while your app is in the foreground or while it’s in the background — for example, by using Background Tasks. When you end a Live Activity, include a final content update using the `content` parameter to ensure the Live Activity shows the latest and final content update after it ends. This is important because the Live Activity may remain visible until the system or the person removes it.

## See Also

### Ending a Live Activity

func end(ActivityContent&lt;Activity&lt;Attributes>.ContentState>?, dismissalPolicy: ActivityUIDismissalPolicy) async

Ends an active Live Activity.

struct ActivityUIDismissalPolicy

The structure that describes when the system should remove a Live Activity that ended.

