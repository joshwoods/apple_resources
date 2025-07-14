

- StoreKit
- ProductIconPhase
-  promotionalIcon 

Instance Property

# promotionalIcon

The promotional image, if the loading task is successful.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var promotionalIcon: Image? { get }
```

## Discussion

This value is `nil` while the image is loading, or if the system can’t access the promotional image for any reason. Use this value as a convenience to access the image in code that doesn’t depend on the reason an image may not be accessible.

For information about setting up promotional images, see Promote in-app purchases.

