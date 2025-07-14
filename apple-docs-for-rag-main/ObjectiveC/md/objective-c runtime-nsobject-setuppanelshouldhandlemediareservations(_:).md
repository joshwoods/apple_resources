

- Objective-C Runtime
- NSObject
-  setupPanelShouldHandleMediaReservations(\_:) 

Instance Method

# setupPanelShouldHandleMediaReservations(\_:)

This delegate method allows the delegate to control how media reservations are handled.

macOS

``` source
func setupPanelShouldHandleMediaReservations(_ aPanel: DRSetupPanel!) -> Bool
```

## Parameters 

`aPanel`  

The setup panel sending the message.

## Return Value

## Discussion

Return `NO` to indicate the delegate will handle media reservations. Return `YES` to indicate the setupPanel should handle media reservations itself.

