

- BrowserEngineKit
- BETextInteraction
-  showReplacements(forText:) 

Instance Method

# showReplacements(forText:)

Displays inline text replacements for the current selection.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func showReplacements(forText text: String)
```

## Overview

Call this method to present system UI for suggesting text replacements, for example, when your browser text view receives promptForReplace(_:).

## See Also

### Text replacements

func addShortcut(forText: String, from: CGRect)

Presents UI for a person to add a text-replacement shortcut to the keyboard dictionary.

