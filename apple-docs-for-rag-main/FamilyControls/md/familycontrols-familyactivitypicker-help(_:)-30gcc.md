

- FamilyControls
- FamilyActivityPicker
-  help(\_:) 

Instance Method

# help(\_:)

Adds help text to a view using a string that you provide.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func help(_ text: S) -> some View where S : StringProtocol
```

## Parameters 

`text`  

The text to use as help.

## Discussion

Adding help to a view configures the view’s accessibility hint and its help tag (also called a *tooltip*) in macOS or visionOS. For more information on using help tags, see Offering help in the Human Interface Guidelines.

```
Image(systemName: "pin.circle")
    .foregroundColor(pointOfInterest.tintColor)
    .help(pointOfInterest.name)
```

## See Also

### Help Text

func help(Text) -> some View

Adds help text to a view using a text view that you provide.

func help(LocalizedStringKey) -> some View

Adds help text to a view using a localized string that you provide.

