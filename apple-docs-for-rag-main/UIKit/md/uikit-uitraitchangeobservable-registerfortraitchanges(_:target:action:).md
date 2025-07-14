

- UIKit
- UITraitChangeObservable
-  registerForTraitChanges(\_:target:action:) 

Instance Method

# registerForTraitChanges(\_:target:action:)

Registers a list of traits to observe, and calls a method on the specified target object when one of the observed traits changes.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@discardableResult @MainActor
func registerForTraitChanges(
    _ traits: [UITrait],
    target: Any,
    action: Selector
) -> any UITraitChangeRegistration
```

**Required**

## Parameters 

`traits`  

An array of traits to observe for changes.

`target`  

The object that receives the method call passed in the action parameter.

`action`  

A selector identifying the method the system calls when one of the registered trait changes.

## Return Value

An opaque token you can use to stop observing trait changes by passing to unregisterForTraitChanges(_:). You don’t have to unregister your observations, and you can safely ignore this value.

## Discussion

The method specified by the selector can take zero, one, or two arguments. If the method takes one argument, the system passes the object whose trait collection is changing. If the method takes two arguments, the system passes the trait collection prior to the observed changes as the second argument.

The following example registers size class traits so that the system executes the closure when a size class trait changes in the view’s trait collection:

```
@objc func sizeClassChanged(view: UIView, previousTraitCollection: UITraitCollection) {
    // Perform invalidation in response to the size class changing.
}

let sizeTraits: [UITrait] = [UITraitVerticalSizeClass.self, UITraitHorizontalSizeClass.self]

view.registerForTraitChanges(sizeTraits, target: self, action: #selector(sizeClassChanged(view:
previousTraitCollection:)))

```

## See Also

### Observing trait changes

func registerForTraitChanges([UITrait], action: Selector) -> any UITraitChangeRegistration

Registers a list of traits to observe, and calls a method on the receiving object when one of the observed traits changes.

**Required**

func registerForTraitChanges&lt;TraitEnvironment>([UITrait], handler: Self.TraitChangeHandler&lt;TraitEnvironment>) -> any UITraitChangeRegistration

Registers a list of traits to observe and a closure to execute when one of the observed traits changes.

**Required**

func unregisterForTraitChanges(any UITraitChangeRegistration)

Tells the system to stop observing previously registered traits.

**Required**

typealias TraitChangeHandler

A closure the system executes when observed traits change.

protocol UITraitChangeRegistration

