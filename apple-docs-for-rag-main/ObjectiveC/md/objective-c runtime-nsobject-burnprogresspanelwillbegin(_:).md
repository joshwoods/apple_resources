

- Objective-C Runtime
- NSObject
-  burnProgressPanelWillBegin(\_:) 

Instance Method

# burnProgressPanelWillBegin(\_:)

Notification sent by the panel before display.

macOS

``` source
func burnProgressPanelWillBegin(_ aNotification: Notification!)
```

## Parameters 

`aNotification`  

Always `DRBurnProgressPanelDidFinishNotification`

## Discussion

If the delegate implements this method it will receive the message immediately before the panel is displayed.

