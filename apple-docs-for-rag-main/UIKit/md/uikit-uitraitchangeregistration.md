

- UIKit
-  UITraitChangeRegistration 

Protocol

# UITraitChangeRegistration

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
protocol UITraitChangeRegistration : NSCopying, NSObjectProtocol
```

## Mentioned in 

Building a desktop-class iPad app

## Relationships

### Inherits From

- NSCopying
- NSObjectProtocol

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

typealias TraitChangeHandler

A closure the system executes when observed traits change.

