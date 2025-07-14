

- UIKit
- UITextPasteDelegate
-  textPasteConfigurationSupporting(\_:transform:) 

Instance Method

# textPasteConfigurationSupporting(\_:transform:)

Tells the delegate to transform the pasted or dropped text item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textPasteConfigurationSupporting(
    _ textPasteConfigurationSupporting: any UITextPasteConfigurationSupporting,
    transform item: any UITextPasteItem
)
```

## Parameters 

`textPasteConfigurationSupporting`  

The object that received the paste or drop request.

`item`  

The text paste item included in the paste or drop operation.

## Discussion

This method is called for each text paste item during a paste or drop operation. You’re required to call one of the `setResult` methods (see Setting a text paste item’s result value) on `item`, but the call doesn’t have to be within the scope of the transform method. It can, for example, be part of the asynchronous handling code for the itemProvider, or it can be part of a completion block. You can make the call whenever you prefer.

It’s safe to use the provided UITextPasteItem object on any thread, but the transform method is always called on the main thread.

