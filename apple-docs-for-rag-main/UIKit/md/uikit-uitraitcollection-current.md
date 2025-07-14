

- UIKit
- UITraitCollection
-  current 

Type Property

# current

The trait collection for the current execution context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
class var current: UITraitCollection { get set }
```

## Discussion

This property provides a way to get a trait collection from the currently updating trait environment when your code doesn’t have direct access to the trait environment. UIKit updates the value of this property before calling the following methods of UIView, UIViewController, and UIPresentationController. Inside these methods, the trait collection contains the traits describing the currently updating view or controller.

The following table lists the supported methods where UIKit sets the current value:

| UIView | UIViewController | UIPresentationController |
|----|----|----|
| draw(_:)  layoutSubviews()  tintColorDidChange()  The `action` method of `UIView/registerForTraitChanges(_:target:action:)`  The `handler` closure of `UIView/registerForTraitChanges(_:handler:)`  traitCollectionDidChange(_:) | viewWillLayoutSubviews()  viewDidLayoutSubviews()  The `action` method of `UIViewController/registerForTraitChanges(_:target:action:)`  The `handler` closure of `UIView/registerForTraitChanges(_:handler:)`  traitCollectionDidChange(_:) | containerViewWillLayoutSubviews()  containerViewDidLayoutSubviews()  The `action` method of `UIPresentationController/registerForTraitChanges(_:target:action:)`  The `handler` closure of `UIPresentationController/registerForTraitChanges(_:handler:)`  traitCollectionDidChange(_:) |

Outside these methods, you’re responsible for ensuring the current property has a valid trait collection. Otherwise, the contents of the collection are undefined. To ensure that current contains a valid trait collection, use one of these techniques:

- Use performAsCurrent(_:) to execute your code inside a context with a valid current property. This is the preferred way to set current.

- Set current to a known good trait collection. If you set current, you need to save and restore the trait environment, as the code example below shows.

UIColor implicitly uses the current trait collection when it resolves a dynamic color to a static color value, such as a CGColor or an RGB value. To resolve a dynamic color, make sure that current contains a valid collection. Alternatively, the method resolvedColor(with:) resolves a color from a given trait collection and doesn’t rely on current.

UIKit stores the value of the current property as a thread-local variable, so access is lightweight and free of side effects. Changing the traits on a nonmain thread doesn’t affect the current traits on your app’s main thread.

Whenever possible, use performAsCurrent(_:) rather than manually setting current. If you need to set current, keep the following in mind:

- Before modifying current, save the value, and restore it after you’re done.

- Always start with a trait collection from a concrete instance of UITraitEnvironment rather than creating a new UITraitCollection instance.

The performAsCurrent(_:) method handles these tasks for you.

The example below sets the current property to resolve a dynamic color into a CGColor:

```
func updateBorderColor(layer: CALayer) {
    let savedTraitCollection = UITraitCollection.current
    // Set the property with a trait collection from a view.
    UITraitCollection.current = view.traitCollection
    // Methods and properties relying on current are safe to use here.
    layer.borderColor = UIColor.label.cgColor
    // Restore the saved collection.
    UITraitCollection.current = savedTraitCollection
}
```

