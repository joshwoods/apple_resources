

- Foundation
- NSUserActivityDelegate
-  userActivityWillSave(\_:) 

Instance Method

# userActivityWillSave(\_:)

Notifies the delegate that the user activity will be saved to be continued or persisted.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func userActivityWillSave(_ userActivity: NSUserActivity)
```

## Parameters 

`userActivity`  

The user activity to update.

## Discussion

The delegate overrides this method to update the activity with current state.

## See Also

### Managing activity continuation

func userActivityWasContinued(NSUserActivity)

Notifies the delegate that the user activity was continued on another device.

