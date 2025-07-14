

- UIKit
- UITextInputStringTokenizer
-  init(textInput:) 

Initializer

# init(textInput:)

Returns an object initialized with the document object that directly communicates with the text input system.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(textInput: any UIResponder & UITextInput)
```

## Parameters 

`textInput`  

The document object in the application that adopts the UITextInput protocol for the purposes of communicating with the text input system.

## Return Value

An instance of a subclass of UITextInputStringTokenizer, or `nil` if the object couldn’t be created.

## Discussion

The subclass of UITextInputStringTokenizer shouldn’t retain `textInput`; the tokenizer should always have a lifetime bounded by that of the UITextInput-conforming object and a retaining reference would create a retain cycle.

