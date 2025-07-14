

- UIKit
- UISheetPresentationController
- UISheetPresentationController.Detent
-  resolvedValue(in:) 

Instance Method

# resolvedValue(in:)

Resolves a detent to its value.

iOS 16.0+iPadOS 16.0+Mac Catalyst

``` source
@MainActor @preconcurrency
func resolvedValue(in context: any UISheetPresentationControllerDetentResolutionContext) -> CGFloat?
```

## Parameters 

`context`  

A context for resolving custom detent values. This context is available in the `resolver` closure of custom(identifier:resolver:).

## Return Value

A CGFloat that represents the value of the detent, or `nil` if the detent is inactive in the provided context.

## Discussion

You can use this method to get the values of the system medium and large detents, or the value of a custom detent. Use this method inside custom(identifier:resolver:) to construct a custom detent according to the values of known detents.

## See Also

### Creating a custom detent

static func custom(identifier: UISheetPresentationController.Detent.Identifier?, resolver: (any UISheetPresentationControllerDetentResolutionContext) -> CGFloat?) -> UISheetPresentationController.Detent

Creates a custom detent for a sheet by computing its value according to the properties of the provided context.

protocol UISheetPresentationControllerDetentResolutionContext

A context for resolving custom detent values.

