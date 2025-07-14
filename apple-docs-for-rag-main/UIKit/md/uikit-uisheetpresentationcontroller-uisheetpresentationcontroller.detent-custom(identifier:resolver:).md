

- UIKit
- UISheetPresentationController
- UISheetPresentationController.Detent
-  custom(identifier:resolver:) 

Type Method

# custom(identifier:resolver:)

Creates a custom detent for a sheet by computing its value according to the properties of the provided context.

iOS 16.0+iPadOS 16.0+Mac Catalyst

``` source
@MainActor @preconcurrency
static func custom(
    identifier: UISheetPresentationController.Detent.Identifier? = nil,
    resolver: @escaping (any UISheetPresentationControllerDetentResolutionContext) -> CGFloat?
) -> UISheetPresentationController.Detent
```

## Parameters 

`identifier`  

An identifier for the detent. Specify a unique identifier for each custom detent for a sheet. If you don’t specify an identifier, the system generates a random identifier.

`resolver`  

A closure for resolving the detent value with an input of type UISheetPresentationControllerDetentResolutionContext. The value you return from this closure is a height within the safe area of the sheet. For example, return `200` for a detent with a height of `200` plus safeAreaInsets.bottom when the sheet is edge-attached, or `200` when the sheet is floating. Return `nil` to specify that the detent is inactive according to the provided context.

If the closure depends on any external inputs, call invalidateDetents() on the sheet when the external inputs change.

Don’t set any properties on UISheetPresentationController during the execution of this closure.

## See Also

### Creating a custom detent

func resolvedValue(in: any UISheetPresentationControllerDetentResolutionContext) -> CGFloat?

Resolves a detent to its value.

protocol UISheetPresentationControllerDetentResolutionContext

A context for resolving custom detent values.

