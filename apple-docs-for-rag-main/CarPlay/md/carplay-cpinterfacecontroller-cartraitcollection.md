

- CarPlay
- CPInterfaceController
-  carTraitCollection 

Instance Property

# carTraitCollection

The trait collection of the vehicle’s primary screen.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var carTraitCollection: UITraitCollection { get }
```

## Discussion

Use this trait collection to derive metrics, such as display scale, for your CarPlay templates. For example, images you display in a CPListTemplate can use this trait collection’s display scale rather than the scale of the user’s iPhone screen.

