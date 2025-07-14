

- FinanceKitUI
- AddOrderToWalletButton
-  activityBackgroundTint(\_:) 

Instance Method

# activityBackgroundTint(\_:)

Sets the tint color for the background of a Live Activity that appears on the Lock Screen.

FinanceKitUISwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor @preconcurrency
func activityBackgroundTint(_ color: Color?) -> some View
```

## Parameters 

`color`  

The background tint color to apply. To use the system’s default background material, pass `nil`.

## Discussion

When you set a custom background tint color, consider setting a custom text color for the auxiliary button people use to end a Live Activity on the Lock Screen. To set a custom text color, use the activitySystemActionForegroundColor(_:) view modifier.

