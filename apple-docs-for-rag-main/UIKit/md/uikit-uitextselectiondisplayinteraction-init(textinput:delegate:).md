

- UIKit
- UITextSelectionDisplayInteraction
-  init(textInput:delegate:) 

Initializer

# init(textInput:delegate:)

Creates a new text selection display interaction object for the specified text view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
init(
    textInput: any UITextInput,
    delegate: any UITextSelectionDisplayInteractionDelegate
)
```

## Parameters 

`textInput`  

The text input view that receives this interaction view.

`delegate`  

An optional delegate object to manage the selection UI views.

