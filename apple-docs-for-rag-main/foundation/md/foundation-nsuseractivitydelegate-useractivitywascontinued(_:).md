

- Foundation
- NSUserActivityDelegate
-  userActivityWasContinued(\_:) 

Instance Method

# userActivityWasContinued(\_:)

Notifies the delegate that the user activity was continued on another device.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func userActivityWasContinued(_ userActivity: NSUserActivity)
```

## Parameters 

`userActivity`  

The user activity that was continued.

## See Also

### Managing activity continuation

func userActivityWillSave(NSUserActivity)

Notifies the delegate that the user activity will be saved to be continued or persisted.

