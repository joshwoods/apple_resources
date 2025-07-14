

- UIKit
- UIPasteConfigurationSupporting
-  paste(itemProviders:) 

Instance Method

# paste(itemProviders:)

Performs a paste operation on the responder object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func paste(itemProviders: [NSItemProvider])
```

## Parameters 

`itemProviders`  

An array of NSItemProvider objects.

## Discussion

This method performs a paste operation on the responder object, pasting the data provided by specified item providers.

## See Also

### Performing a paste operation

func canPaste([NSItemProvider]) -> Bool

Returns a Boolean value that determines whether the responder object can perform a paste operation using data provided by the item providers.

