

- UIKit
- UITextSelectionDisplayInteraction
-  textInput 

Instance Property

# textInput

The text input object that manages the selection.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
weak var textInput: (any UITextInput)? { get }
```

## Mentioned in 

Adopting system selection UI in custom text views

## Discussion

Use this property to refer to the text input view that manages the text selection. You specify this view when you create the UITextSelectionDisplayInteraction object.

