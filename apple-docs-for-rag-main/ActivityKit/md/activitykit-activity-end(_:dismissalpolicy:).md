

- ActivityKit
- Activity
-  end(\_:dismissalPolicy:) 

Instance Method

# end(\_:dismissalPolicy:)

Ends an active Live Activity.

iOS 16.2+iPadOS 16.2+

``` source
func end(
    _ content: ActivityContent.ContentState>?,
    dismissalPolicy: ActivityUIDismissalPolicy = .default
) async
```

## Parameters 

`content`  

The latest and final dynamic content for the Live Activity that ended. The size of the encoded content can’t exceed 4KB in size.

`dismissalPolicy`  

Describes how and when the system should dismiss a Live Activity and and remove it from the Lock Screen.

## Mentioned in 

Displaying live data with Live Activities

## Discussion

End an active Live Activity while your app is in the foreground or while it’s in the background — for example, by using Background Tasks. When you end a Live Activity, include a final content update using the `content` parameter to ensure the Live Activity shows the latest and final content update after it ends. This is important because the Live Activity may remain visible until the system or the person removes it.

## See Also

### Ending a Live Activity

struct ActivityUIDismissalPolicy

The structure that describes when the system should remove a Live Activity that ended.

func end(ActivityContent&lt;Activity&lt;Attributes>.ContentState>?, dismissalPolicy: ActivityUIDismissalPolicy, timestamp: Date) async

Ends an active Live Activity.

