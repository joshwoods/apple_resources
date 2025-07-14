

- UIKit
- UITraitChangeObservable
-  registerForTraitChanges(\_:action:) 

Instance Method

# registerForTraitChanges(\_:action:)

Registers a list of traits to observe, and calls a method on the receiving object when one of the observed traits changes.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@discardableResult @MainActor
func registerForTraitChanges(
    _ traits: [UITrait],
    action: Selector
) -> any UITraitChangeRegistration
```

**Required**

## Parameters 

`traits`  

An array of traits to observe for changes.

`action`  

A selector identifying the method the system calls when one of the registered trait changes.

## Return Value

An opaque token you can use to stop observing trait changes by passing to unregisterForTraitChanges(_:). You don’t have to unregister your observations, and you can safely ignore this value.

## Discussion

This is a convenience method for registerForTraitChanges(_:target:action:) when the object receiving the registration is the target of the action. For example, when you register for changes on `self`, the `target` is `self`.

The following example calls setNeedsLayout() in response to changes to size traits:

```
let sizeTraits: [UITrait] = [UITraitVerticalSizeClass.self, UITraitHorizontalSizeClass.self]

// Register for size class changes on self, and invalidate the layout in response to changes.
registerForTraitChanges(sizeTraits, action: #selector(UIView.setNeedsLayout))
```

## See Also

### Observing trait changes

func registerForTraitChanges&lt;TraitEnvironment>([UITrait], handler: Self.TraitChangeHandler&lt;TraitEnvironment>) -> any UITraitChangeRegistration

Registers a list of traits to observe and a closure to execute when one of the observed traits changes.

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

