

- UIKit
- UIPasteConfigurationSupporting
-  canPaste(\_:) 

Instance Method

# canPaste(\_:)

Returns a Boolean value that determines whether the responder object can perform a paste operation using data provided by the item providers.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func canPaste(_ itemProviders: [NSItemProvider]) -> Bool
```

## Parameters 

`itemProviders`  

An array of NSItemProvider objects.

## Return Value

true if the responder object can perform a paste operation using specified item providers; otherwise, false.

## See Also

### Performing a paste operation

func paste(itemProviders: [NSItemProvider])

Performs a paste operation on the responder object.

