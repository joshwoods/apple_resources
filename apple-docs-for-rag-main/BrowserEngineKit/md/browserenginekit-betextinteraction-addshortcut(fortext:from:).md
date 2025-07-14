

- BrowserEngineKit
- BETextInteraction
-  addShortcut(forText:from:) 

Instance Method

# addShortcut(forText:from:)

Presents UI for a person to add a text-replacement shortcut to the keyboard dictionary.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func addShortcut(
    forText text: String,
    from presentationRect: CGRect
)
```

## See Also

### Text replacements

func showReplacements(forText: String)

Displays inline text replacements for the current selection.

