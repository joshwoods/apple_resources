

- BrowserEngineKit
- BEResponderEditActions
-  replace(\_:) 

Instance Method

# replace(\_:)

Removes the selected text and inputs the chosen replacement text.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
optional func replace(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Overview

To invoke the standard operating system behavior for replacing text, call textInput(_:deferReplaceTextActionToSystem:) in your implementation of this method.

## See Also

### Finding and replacing text

func findSelected(Any?)

Begins a search for the selected content in your browser text view.

func promptForReplace(Any?)

Shows potential replacements for the selected content.

func addShortcut(Any?)

Adds a text-replacement shortcut to the edit dictionary.

