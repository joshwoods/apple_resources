

- UIKit
- UITraitChangeObservable
-  UITraitChangeObservable.TraitChangeHandler 

Type Alias

# UITraitChangeObservable.TraitChangeHandler

A closure the system executes when observed traits change.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
typealias TraitChangeHandler = (TraitEnvironment, UITraitCollection) -> Void where TraitEnvironment : UITraitEnvironment
```

## Parameters 

`traitEnvironment`  

The observed object containing the updated trait collection.

`previousTraitCollection`  

The trait collection prior to the changes that triggered the execution of the handler.

## Discussion

Use registerForTraitChanges(_:handler:) to register a list of traits to observe and a handler to execute.

If the closure captures a strong reference to the object receiving the registration, it creates a strong reference cycle. Use the `traitEnvironment` parameter to refer to the observed object inside the closure.

## See Also

### Observing trait changes

func registerForTraitChanges([UITrait], action: Selector) -> any UITraitChangeRegistration

Registers a list of traits to observe, and calls a method on the receiving object when one of the observed traits changes.

**Required**

func registerForTraitChanges&lt;TraitEnvironment>([UITrait], handler: Self.TraitChangeHandler&lt;TraitEnvironment>) -> any UITraitChangeRegistration

Registers a list of traits to observe and a closure to execute when one of the observed traits changes.

**Required**

func registerForTraitChanges([UITrait], target: Any, action: Selector) -> any UITraitChangeRegistration

Registers a list of traits to observe, and calls a method on the specified target object when one of the observed traits changes.

**Required**

func unregisterForTraitChanges(any UITraitChangeRegistration)

Tells the system to stop observing previously registered traits.

**Required**

protocol UITraitChangeRegistration

