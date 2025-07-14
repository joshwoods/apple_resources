

- Objective-C Runtime
- NSObject
-  eraseProgressPanelDidFinish(\_:) 

Instance Method

# eraseProgressPanelDidFinish(\_:)

Notification sent by the panel after ordering out.

macOS

``` source
func eraseProgressPanelDidFinish(_ aNotification: Notification!)
```

## Parameters 

`aNotification`  

Always `DREraseProgressPanelDidFinishNotification` You can retrieve the `DREraseProgressPanel` object in question by sending object to `aNotification`.

## Discussion

If the delegate implements this method it will receive the message after the panel is removed from display.

