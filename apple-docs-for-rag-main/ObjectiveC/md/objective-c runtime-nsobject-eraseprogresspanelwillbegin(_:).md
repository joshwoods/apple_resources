

- Objective-C Runtime
- NSObject
-  eraseProgressPanelWillBegin(\_:) 

Instance Method

# eraseProgressPanelWillBegin(\_:)

Notification sent by the panel before display.

macOS

``` source
func eraseProgressPanelWillBegin(_ aNotification: Notification!)
```

## Parameters 

`aNotification`  

Always `DREraseProgressPanelWillBeginNotification` You can retrieve the `DREraseProgressPanel` object in question by sending object to `aNotification`.

## Discussion

If the delegate implements this method it will receive the message immediately before the panel is displayed.

