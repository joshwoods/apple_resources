

- BrowserEngineKit
- BEResponderEditActions
-  promptForReplace(\_:) 

Instance Method

# promptForReplace(\_:)

Shows potential replacements for the selected content.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
optional func promptForReplace(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Overview

To present the standard operating system UI for this action, call showReplacements(forText:) in your implementation of this method.

## See Also

### Finding and replacing text

func findSelected(Any?)

Begins a search for the selected content in your browser text view.

func replace(Any?)

Removes the selected text and inputs the chosen replacement text.

func addShortcut(Any?)

Adds a text-replacement shortcut to the edit dictionary.

