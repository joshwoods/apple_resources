

- Network Extension
-  NEHotspotHelperHandler 

Type Alias

# NEHotspotHelperHandler

The type definition for the Hotspot Helper’s command handler block.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
typealias NEHotspotHelperHandler = (NEHotspotHelperCommand) -> Void
```

## Discussion

The Hotspot Helper app provides a block of this type when it invokes the `registerWithOptions:queue:handler:` method.

The block is invoked every time there is a command to be processed.

## See Also

### Registering a hotspot helper

class func register(options: [String : NSObject]?, queue: dispatch_queue_t, handler: NEHotspotHelperHandler) -> Bool

Register the application as a Hotspot Helper.

let kNEHotspotHelperOptionDisplayName: String

The string displayed in Wi-Fi Settings for a network handled by the application.

