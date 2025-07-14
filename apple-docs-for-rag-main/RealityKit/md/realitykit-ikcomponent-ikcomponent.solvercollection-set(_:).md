

- RealityKit
- IKComponent
- IKComponent.SolverCollection
-  set(\_:) 

Instance Method

# set(\_:)

Updates the element with identifier matching the new value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult
mutating func set(_ newValue: IKComponent.SolverCollection.Element) -> IKComponent.SolverCollection.Element?
```

## Parameters 

`newValue`  

The new value to store.

## Return Value

The previous value if the identifier was found, nil otherwise.

