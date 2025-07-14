

- BrowserEngineKit
- BEResponderEditActions
-  findSelected(\_:) 

Instance Method

# findSelected(\_:)

Begins a search for the selected content in your browser text view.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
optional func findSelected(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Overview

UIKit calls this method when someone selects Use Selection for Find from an editing menu. Present the UI for finding text in your view, and use the selected text for the search. To present the standard operating system UI for finding text, and support standard keyboard shortcuts, add a UIFindInteraction to your browser text view.

## See Also

### Finding and replacing text

func promptForReplace(Any?)

Shows potential replacements for the selected content.

func replace(Any?)

Removes the selected text and inputs the chosen replacement text.

func addShortcut(Any?)

Adds a text-replacement shortcut to the edit dictionary.

