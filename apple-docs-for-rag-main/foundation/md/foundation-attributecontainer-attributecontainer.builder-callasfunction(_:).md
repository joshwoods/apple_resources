

- Foundation
- AttributeContainer
- AttributeContainer.Builder
-  callAsFunction(\_:) 

Instance Method

# callAsFunction(\_:)

Builds an attribute container by setting an attribute and returning a modified attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
func callAsFunction(_ value: T.Value) -> AttributeContainer where T.Value : Sendable
```

## Parameters 

`value`  

The value to set on the returned attribute container.

## Return Value

An attribute container with the provided value set on the builder’s AttributedStringKey.

