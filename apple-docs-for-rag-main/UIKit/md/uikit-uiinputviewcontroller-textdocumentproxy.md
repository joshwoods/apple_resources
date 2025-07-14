

- UIKit
- UIInputViewController
-  textDocumentProxy 

Instance Property

# textDocumentProxy

A proxy to the text input object that the custom keyboard is interacting with.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var textDocumentProxy: any UITextDocumentProxy { get }
```

## Mentioned in 

Configuring a custom keyboard interface

## Discussion

This property conforms directly or indirectly to the following protocols:

- The UITextDocumentProxy protocol provides textual context around the insertion point

- The UIKeyInput protocol provides the insert and delete methods, and lets you find out if the text object is empty

- The UITextInputTraits protocol provides insight into the characteristics of the text input object, such as whether it requests a style of autocapitalization and which sort of keyboard it expects (for example, email address, URL, number pad, or default).

Employ this property to interact with the current text input object. For example, to insert text you would write code like this:

```
[self.textDocumentProxy insertText:@"hello "]; // Inserts the string "hello " at the insertion point
```

To delete text, you’d write code like this:

```
[self.textDocumentProxy deleteBackward];       // Deletes the character to the left of the insertion point
```

## See Also

### Interacting with a text input object

protocol UITextDocumentProxy

An object that provides textual context to a custom keyboard.

