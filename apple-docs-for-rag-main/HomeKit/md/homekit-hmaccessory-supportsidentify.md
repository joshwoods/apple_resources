

- HomeKit
- HMAccessory
-  supportsIdentify 

Instance Property

# supportsIdentify

A Boolean value that indicates whether the accessory supports the identify action.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+tvOS 11.3+visionOS 1.0+watchOS 4.3+

``` source
var supportsIdentify: Bool { get }
```

## Discussion

If false, any calls to the identify(completionHandler:) method return an error. However, even if this property is true, calls to identify(completionHandler:) may not succeed.

## See Also

### Asking an accessory to identify itself

func identify(completionHandler: ((any Error)?) -> Void)

Asks an accessory to identify itself.

