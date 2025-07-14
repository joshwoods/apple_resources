

- FamilyControls
- FamilyActivityIconView
-  autocorrectionDisabled(\_:) 

Instance Method

# autocorrectionDisabled(\_:)

Sets whether to disable autocorrection for this view.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 8.0+

``` source
nonisolated
func autocorrectionDisabled(_ disable: Bool = true) -> some View
```

## Parameters 

`disable`  

A Boolean value that indicates whether autocorrection is disabled for this view. The default value is `true`.

## Discussion

Use this method when the effect of autocorrection would make it more difficult for the user to input information. The entry of proper names and street addresses are examples where autocorrection can negatively affect the user’s ability complete a data entry task.

The example below configures a `TextField` with the default keyboard. Disabling autocorrection allows the user to enter arbitrary text without the autocorrection system offering suggestions or attempting to override their input.

```
TextField("1234 Main St.", text: $address)
    .keyboardType(.default)
    .autocorrectionDisabled(true)
```

