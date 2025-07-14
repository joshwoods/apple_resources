

- Network Extension
- NEHotspotHelper
-  register(options:queue:handler:) 

Type Method

# register(options:queue:handler:)

Register the application as a Hotspot Helper.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func register(
    options: [String : NSObject]? = nil,
    queue: dispatch_queue_t,
    handler: @escaping NEHotspotHelperHandler
) -> Bool
```

## Parameters 

`options`  

If not nil, a NSDictionary containing `kNEHotspotHelperOption*` keys (currently just `kNEHotspotHelperOptionDisplayName`).

`queue`  

The dispatch_queue_t to invoke the handle block on.

`handler`  

The `NEHotspotHelperHandler` block to execute to process helper commands.

## Return Value

true if the registration was successful, false otherwise

## Discussion

Once this API is invoked successfully, the application becomes eligible to be launched in the background and participate in various hotspot related functions.

This method should be called once when the application starts up. Invoking it again will have no effect and result in false being returned.

Warning

The application’s `Info.plist` must include a `UIBackgroundModes` array containing `network-authentication`.

Warning

The application must set `com.apple.developer.networking.HotspotHelper` as one of its entitlements. The value of the entitlement is a boolean set to `true`.

## See Also

### Registering a hotspot helper

let kNEHotspotHelperOptionDisplayName: String

The string displayed in Wi-Fi Settings for a network handled by the application.

typealias NEHotspotHelperHandler

The type definition for the Hotspot Helper’s command handler block.

