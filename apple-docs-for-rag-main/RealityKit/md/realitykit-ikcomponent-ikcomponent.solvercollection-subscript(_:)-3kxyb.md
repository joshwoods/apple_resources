

- RealityKit
- IKComponent
- IKComponent.SolverCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element with the specified identifier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
subscript(id: IKComponent.SolverCollection.Element.ID) -> IKComponent.SolverCollection.Element? { get set }
```

## Parameters 

`id`  

The identifier of the requested element.

## Overview

The following set scenarios are ignored:

- Setting nil

- Setting element with different id, e.g. \`collection\[ID(2)\]?.id = ID(3)

- Setting element with id not in the set

