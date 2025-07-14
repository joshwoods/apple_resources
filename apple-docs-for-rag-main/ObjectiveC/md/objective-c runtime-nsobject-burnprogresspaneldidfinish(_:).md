

- Objective-C Runtime
- NSObject
-  burnProgressPanelDidFinish(\_:) 

Instance Method

# burnProgressPanelDidFinish(\_:)

Notification sent by the panel after ordering out.

macOS

``` source
func burnProgressPanelDidFinish(_ aNotification: Notification!)
```

## Parameters 

`aNotification`  

Always `DRBurnProgressPanelDidFinishNotification`

## Discussion

If the delegate implements this method it will receive the message after the panel is removed from display.

