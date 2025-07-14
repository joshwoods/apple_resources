

- FamilyControls
- FamilyActivityTitleView
-  autocapitalization(\_:) 

Instance Method

# autocapitalization(\_:)

Sets whether to apply auto-capitalization to this view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0+visionOS 1.0+

``` source
nonisolated
func autocapitalization(_ style: UITextAutocapitalizationType) -> some View
```

## Parameters 

`style`  

One of the autocapitalization modes defined in the UITextAutocapitalizationType enumeration.

## Discussion

Use `autocapitalization(_:)` when you need to automatically capitalize words, sentences, or other text like proper nouns.

In example below, as the user enters text each word is automatically capitalized:

```
TextField("Last, First", text: $fullName)
    .autocapitalization(UITextAutocapitalizationType.words)
```

The UITextAutocapitalizationType enumeration defines the available capitalization modes. The default is UITextAutocapitalizationType.sentences.

