

- Journaling Suggestions
- JournalingSuggestionsPicker
-  disableAutocorrection(\_:) 

Instance Method

# disableAutocorrection(\_:)

Sets whether to disable autocorrection for this view.

Journaling SuggestionsSwiftUIiOS 13.0–18.4DeprecatedmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func disableAutocorrection(_ disable: Bool?) -> some View
```

## Parameters 

`enabled`  

A Boolean value that indicates whether autocorrection is disabled for this view.

## Discussion

Use `disableAutocorrection(_:)` when the effect of autocorrection would make it more difficult for the user to input information. The entry of proper names and street addresses are examples where autocorrection can negatively affect the user’s ability complete a data entry task.

In the example below configures a `TextField` with the `.default` keyboard. Disabling autocorrection allows the user to enter arbitrary text without the autocorrection system offering suggestions or attempting to override their input.

```
TextField("1234 Main St.", text: $address)
    .keyboardType(.default)
    .disableAutocorrection(true)
```

