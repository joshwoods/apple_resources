

- RealityKit
- IKRig
- IKRig.JointCollection
-  set(\_:) 

Instance Method

# set(\_:)

Updates the element with identifier matching the provided value’s identifier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult
mutating func set(_ newValue: IKRig.JointCollection.Element) -> IKRig.JointCollection.Element?
```

## Parameters 

`newValue`  

The new element value to store.

## Return Value

The previous element value if the identifier exists, `nil` otherwise.

## Discussion

If an element with the provided identifier is not contained - does nothing.

