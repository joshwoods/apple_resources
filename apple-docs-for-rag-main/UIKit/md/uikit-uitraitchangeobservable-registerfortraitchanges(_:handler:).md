

- UIKit
- UITraitChangeObservable
-  registerForTraitChanges(\_:handler:) 

Instance Method

# registerForTraitChanges(\_:handler:)

Registers a list of traits to observe and a closure to execute when one of the observed traits changes.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@discardableResult @MainActor
func registerForTraitChanges(
    _ traits: [UITrait],
    handler: @escaping Self.TraitChangeHandler
) -> any UITraitChangeRegistration where TraitEnvironment : UITraitEnvironment
```

**Required**

## Parameters 

`traits`  

An array of traits to observe for changes.

`handler`  

A closure that the system executes when one of the registered traits changes.

## Return Value

An opaque token you can use to stop observing trait changes by passing to unregisterForTraitChanges(_:). You don’t have to unregister your observations, and you can safely ignore this value.

## Discussion

The first parameter of the closure provides access to the observed object whose traits have changed, so you don’t need to create a weak reference. When registering for changes on self, use `self` as the name and `Self` as the type of the first parameter.

The following example registers size class traits so that the system executes the closure when a size class trait changes in the view’s trait collection:

```
let sizeTraits: [UITrait] = [UITraitVerticalSizeClass.self, UITraitHorizontalSizeClass.self]

// Register for size class changes on self. Declare the first paramteter as `self: Self`.
// Declaring self as the first parameter eliminates the need to capture self from outside the closure, and avoids strong reference cycles.
registerForTraitChanges(sizeTraits) { (self: Self, previousTraitCollection: UITraitCollection) in
    // Handle the trait change.
}

// Register for size class changes on a different view of class MyView.
view.registerForTraitChanges(sizeTraits) { (view: MyView, previousTraitCollection: UITraitCollection) in
    // Handle the trait change.
}
```

## See Also

### Observing trait changes

func registerForTraitChanges([UITrait], action: Selector) -> any UITraitChangeRegistration

Registers a list of traits to observe, and calls a method on the receiving object when one of the observed traits changes.

**Required**

func registerForTraitChanges([UITrait], target: Any, action: Selector) -> any UITraitChangeRegistration

Registers a list of traits to observe, and calls a method on the specified target object when one of the observed traits changes.

**Required**

func unregisterForTraitChanges(any UITraitChangeRegistration)

Tells the system to stop observing previously registered traits.

**Required**

typealias TraitChangeHandler

A closure the system executes when observed traits change.

protocol UITraitChangeRegistration

