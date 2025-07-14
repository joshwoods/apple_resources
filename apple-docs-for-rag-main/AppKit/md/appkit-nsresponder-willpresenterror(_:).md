

- AppKit
- NSResponder
-  willPresentError(\_:) 

Instance Method

# willPresentError(\_:)

Returns a custom version of the supplied error object that’s more suitable for presentation in alert sheets and dialogs.

macOS

``` source
@MainActor
func willPresentError(_ error: any Error) -> any Error
```

## Parameters 

`error`  

The error object to customize.

## Return Value

The customized error object; if you decide not to customize the error presentation, return by sending this message to `super` (that is, `return [super willPresentError:error]`).

## Discussion

When overriding this method, you can examine `error` and, if its localized description or recovery information is unhelpfully generic, return an error object with more specific localized text. If you do this, always use the domain and error code of the NSError object to distinguish between errors whose presentation you want to customize and those you don’t. Don’t make decisions based on the localized description, recovery suggestion, or recovery options because parsing localized text is problematic.

The default implementation of this method returns `error` unchanged.

## See Also

### Presenting and Customizing Error Information

func presentError(any Error) -> Bool

Presents an error alert to the user as an application-modal dialog.

func presentError(any Error, modalFor: NSWindow, delegate: Any?, didPresent: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents an error alert to the user as a document-modal sheet attached to document window.

