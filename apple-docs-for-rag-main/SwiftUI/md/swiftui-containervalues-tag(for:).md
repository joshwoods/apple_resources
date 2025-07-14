

- SwiftUI
- ContainerValues
-  tag(for:) 

Instance Method

# tag(for:)

The tag value for the given type if the container values contains one.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func tag(for type: V.Type) -> V? where V : Hashable
```

## Parameters 

`type`  

The type to get the tag value for.

## Return Value

The tag value for the given type if the subview has one, otherwise `nil`.

## Discussion

Tag values are set using the `View/tag` modifier.

