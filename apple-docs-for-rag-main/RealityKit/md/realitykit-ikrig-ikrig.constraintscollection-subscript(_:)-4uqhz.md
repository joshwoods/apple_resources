

- RealityKit
- IKRig
- IKRig.ConstraintsCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element with the specified identifier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
subscript(id: IKRig.ConstraintsCollection.Element.ID) -> IKRig.ConstraintsCollection.Element? { get set }
```

## Parameters 

`id`  

The identifier of the requested element.

## Overview

Note

Set `nil` to remove the element with matching identifier.

