

- FinanceKitUI
- AddOrderToWalletButton
-  backgroundPreferenceValue(\_:alignment:\_:) 

Instance Method

# backgroundPreferenceValue(\_:alignment:\_:)

Reads the specified preference value from the view, using it to produce a second view that is applied as the background of the original view.

FinanceKitUISwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
nonisolated
func backgroundPreferenceValue(
    _ key: K.Type,
    alignment: Alignment = .center,
    @ViewBuilder _ transform: @escaping (K.Value) -> V
) -> some View where K : PreferenceKey, V : View
```

## Parameters 

`key`  

The preference key type whose value is to be read.

`alignment`  

An optional alignment to use when positioning the background view relative to the original view.

`transform`  

A function that produces the background view from the preference value read from the original view.

## Return Value

A view that layers a second view behind the view.

## Discussion

The values of the preference key from both views are combined and made visible to the parent view.

