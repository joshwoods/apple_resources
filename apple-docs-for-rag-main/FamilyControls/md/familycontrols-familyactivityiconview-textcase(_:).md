

- FamilyControls
- FamilyActivityIconView
-  textCase(\_:) 

Instance Method

# textCase(\_:)

Sets a transform for the case of the text contained in this view when displayed.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func textCase(_ textCase: Text.Case?) -> some View
```

## Parameters 

`textCase`  

One of the `Text/Case` enumerations; the default is `nil`.

## Return Value

A view that transforms the case of the text.

## Discussion

The default value is `nil`, displaying the text without any case changes.

