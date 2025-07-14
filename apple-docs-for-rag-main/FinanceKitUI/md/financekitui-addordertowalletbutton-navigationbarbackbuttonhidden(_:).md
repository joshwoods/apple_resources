

- FinanceKitUI
- AddOrderToWalletButton
-  navigationBarBackButtonHidden(\_:) 

Instance Method

# navigationBarBackButtonHidden(\_:)

Hides the navigation bar back button for the view.

FinanceKitUISwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func navigationBarBackButtonHidden(_ hidesBackButton: Bool = true) -> some View
```

## Parameters 

`hidesBackButton`  

A Boolean value that indicates whether to hide the back button. The default value is `true`.

## Discussion

Use `navigationBarBackButtonHidden(_:)` to hide the back button for this view.

This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

