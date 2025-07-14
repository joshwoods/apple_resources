

- Core Animation
- CALayer
-  actions 

Instance Property

# actions

A dictionary containing layer actions.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var actions: [String : any CAAction]? { get set }
```

## Discussion

The default value of this property is `nil`. You can use this dictionary to store custom actions for your layer. The contents of this dictionary searched as part of the standard implementation of the action(forKey:) method.

## See Also

### Getting the Layer’s Actions

func action(forKey: String) -> (any CAAction)?

Returns the action object assigned to the specified key.

class func defaultAction(forKey: String) -> (any CAAction)?

Returns the default action for the current class.

