

- Network Extension
- NEHotspotHelper
-  logoff(\_:) 

Type Method

# logoff(\_:)

Terminate the authentication session for a Hotspot network.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func logoff(_ network: NEHotspotNetwork) -> Bool
```

## Parameters 

`network`  

A NEHotspotNetwork corresponding to the currently associated Wi-Fi network.

## Return Value

true if the logoff command was successfully queued, false otherwise.

## Discussion

The application invokes this method when it wants to log off from the current network. Invoking this method causes an NEHotspotHelperCommand of type NEHotspotHelperCommandType.logoff to be issued to the application’s ‘handler’ block, which is registered with the system by calling `NEHotspotHelper registerWithOptions:queue:handler`.

The `network` parameter must correspond to the currently associated Wi-Fi network i.e. it must have come from the `network` property of the NEHotspotHelperCommand or from the `supportedInterfaces` method.

Warning

The application must not actually log off from the network until it receives the command to log off.

