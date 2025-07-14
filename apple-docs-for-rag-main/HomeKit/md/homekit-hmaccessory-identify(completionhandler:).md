

- HomeKit
- HMAccessory
-  identify(completionHandler:) 

Instance Method

# identify(completionHandler:)

Asks an accessory to identify itself.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
func identify(completionHandler completion: @escaping ((any Error)?) -> Void)
```

``` source
func identify() async throws
```

## Parameters 

`completion`  

Block that is invoked once the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

Accessories typically identify themselves by briefly doing something the user can see or hear. The behavior is specific to the device. For example, a light bulb might identify itself by briefly turning on if it is currently off, or by briefly dimming if it is currently on. This can help a user pinpoint one device among several that are similar.

## See Also

### Asking an accessory to identify itself

var supportsIdentify: Bool

A Boolean value that indicates whether the accessory supports the identify action.

