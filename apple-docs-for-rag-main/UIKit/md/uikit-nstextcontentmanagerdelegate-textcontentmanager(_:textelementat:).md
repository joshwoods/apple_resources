

- UIKit
- NSTextContentManagerDelegate
-  textContentManager(\_:textElementAt:) 

Instance Method

# textContentManager(\_:textElementAt:)

The method the framework calls to return the text element at a specific location.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
optional func textContentManager(
    _ textContentManager: NSTextContentManager,
    textElementAt location: any NSTextLocation
) -> NSTextElement?
```

## Parameters 

`textContentManager`  

The content manager.

`location`  

The location of the element.

## Return Value

An NSTextElement.

## Discussion

When non-`nil`, `textContentManager` uses the text element you specify instead of creating one based on its standard mapping logic.

