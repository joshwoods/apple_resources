

- AppKit
- NSTextContentManagerDelegate
-  textContentManager(\_:shouldEnumerate:options:) 

Instance Method

# textContentManager(\_:shouldEnumerate:options:)

Returns a Boolean value that indicates whether the framework should skip this text element in the enumeration.

macOS 12.0+

``` source
optional func textContentManager(
    _ textContentManager: NSTextContentManager,
    shouldEnumerate textElement: NSTextElement,
    options: NSTextContentManager.EnumerationOptions = []
) -> Bool
```

## Parameters 

`textContentManager`  

The content manager.

`textElement`  

The NSTextElement to evaluate.

`options`  

One of the available `NSTextElementProviderEnumerationOptions` options.

## Return Value

A Boolean value that informs the framework to skip this `textElement` in the enumeration. Returning `false` indicates `textElement` to be skipped; otherwise the element is included in the enumeration.

