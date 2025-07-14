

- ActivityKit
- Activity
-  update(\_:alertConfiguration:) 

Instance Method

# update(\_:alertConfiguration:)

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

iOS 16.2+iPadOS 16.2+

``` source
func update(
    _ content: ActivityContent.ContentState>,
    alertConfiguration: AlertConfiguration? = nil
) async
```

## Parameters 

`content`  

The updated dynamic content for the Live Activity. The size of its state property can’t exceed 4KB in size.

`alertConfiguration`  

The alert configuration you use to configure how the system notifies a person about the updated content of the Live Activity.

## Mentioned in 

Displaying live data with Live Activities

## Discussion

The system ignores updates to a Live Activity that’s in the ActivityState.ended state.

## See Also

### Updating a Live Activity

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>) async

Updates the dynamic content of the Live Activity.

struct AlertConfiguration

A structure you use to configure an alert that appears when you update your Live Activity.

func update(using: Activity&lt;Attributes>.ContentState) async

Updates the dynamic content of the Live Activity.

Deprecated

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>, alertConfiguration: AlertConfiguration?, timestamp: Date) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

