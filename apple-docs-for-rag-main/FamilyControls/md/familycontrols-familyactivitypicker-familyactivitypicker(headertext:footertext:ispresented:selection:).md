

- FamilyControls
- FamilyActivityPicker
-  familyActivityPicker(headerText:footerText:isPresented:selection:) 

Instance Method

# familyActivityPicker(headerText:footerText:isPresented:selection:)

Presents an activity picker view as a sheet.

FamilyControlsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor @preconcurrency
func familyActivityPicker(
    headerText: String? = nil,
    footerText: String? = nil,
    isPresented: Binding,
    selection: Binding
) -> some View
```

## Parameters 

`headerText`  

An optional string that provides text for the header of the picker view.

`footerText`  

An optional string that provides text for the footer of the picker view.

`isPresented`  

A binding that indicates whether the app presents the picker view.

`selection`  

A binding that manages the user-selected categories, apps, and web domains.

## Discussion

Use this view modifier to present a FamilyActivityPicker.

