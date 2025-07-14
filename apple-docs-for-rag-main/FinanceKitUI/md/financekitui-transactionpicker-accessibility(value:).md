

- FinanceKitUI
- TransactionPicker
-  accessibility(value:) 

Instance Method

# accessibility(value:)

Adds a textual description of the value that the view contains.

FinanceKitUISwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func accessibility(value: Text) -> ModifiedContent
```

## Discussion

Use this method to describe the value represented by a view, but only if that’s different than the view’s label. For example, for a slider that you label as “Volume” using accessibility(label:), you can provide the current volume setting, like “60%”, using accessibility(value:).

