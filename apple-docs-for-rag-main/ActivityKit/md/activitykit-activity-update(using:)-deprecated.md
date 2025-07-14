

- ActivityKit
- Activity
-  update(using:) Deprecated

Instance Method

# update(using:)

Updates the dynamic content of the Live Activity.

iOS 16.1–16.2DeprecatediPadOS 16.1–16.2Deprecated

``` source
func update(using contentState: Activity.ContentState) async
```

Deprecated

Use update(\_:) instead

## Parameters 

`contentState`  

The updated dynamic content for the Live Activity. The size of the encoded content can’t exceed 4KB in size.

## Discussion

Use this function to update the Live Activity while your app is in the foreground or while it’s in the background — for example, by using Background Tasks.

Note

The system ignores attempts to update a Live Activity that ended.

## See Also

### Updating a Live Activity

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>) async

Updates the dynamic content of the Live Activity.

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>, alertConfiguration: AlertConfiguration?) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

struct AlertConfiguration

A structure you use to configure an alert that appears when you update your Live Activity.

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>, alertConfiguration: AlertConfiguration?, timestamp: Date) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

