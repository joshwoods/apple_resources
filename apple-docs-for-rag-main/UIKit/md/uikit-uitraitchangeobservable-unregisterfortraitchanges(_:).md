

- UIKit
- UITraitChangeObservable
-  unregisterForTraitChanges(\_:) 

Instance Method

# unregisterForTraitChanges(\_:)

Tells the system to stop observing previously registered traits.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor
func unregisterForTraitChanges(_ registration: any UITraitChangeRegistration)
```

**Required**

## Parameters 

`registration`  

A token that identifies the registration, obtained from one of the trait registration method calls.

## Discussion

Use this method if you want the system to stop observing trait changes for a previous registration. UIKit doesn’t require you to unregister for trait changes at the end of the view lifecycle. Unregister only if you need to dynamically change which traits you observe.

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

typealias TraitChangeHandler

A closure the system executes when observed traits change.

protocol UITraitChangeRegistration

