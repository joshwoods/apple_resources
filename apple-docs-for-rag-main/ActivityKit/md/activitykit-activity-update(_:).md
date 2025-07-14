

- ActivityKit
- Activity
-  update(\_:) 

Instance Method

# update(\_:)

Updates the dynamic content of the Live Activity.

iOS 16.2+iPadOS 16.2+

``` source
func update(_ content: ActivityContent.ContentState>) async
```

## Parameters 

`content`  

The updated dynamic content for the Live Activity. The size of its state property can’t exceed 4KB in size.

## Mentioned in 

Displaying live data with Live Activities

## Discussion

Use this function to update the Live Activity while your app is in the foreground or while it’s in the background — for example, by using Background Tasks.

Note

The system ignores attempts to update a Live Activity that ended.

## See Also

### Updating a Live Activity

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>, alertConfiguration: AlertConfiguration?) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

struct AlertConfiguration

A structure you use to configure an alert that appears when you update your Live Activity.

func update(using: Activity&lt;Attributes>.ContentState) async

Updates the dynamic content of the Live Activity.

Deprecated

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>, alertConfiguration: AlertConfiguration?, timestamp: Date) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

