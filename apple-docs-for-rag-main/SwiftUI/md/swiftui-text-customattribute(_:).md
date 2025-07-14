

- SwiftUI
- Text
-  customAttribute(\_:) 

Instance Method

# customAttribute(\_:)

Adds a custom attribute to the text view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func customAttribute(_ value: T) -> Text where T : TextAttribute
```

## Parameters 

`value`  

The attribute to attach.

## Return Value

A version of the text view with `value` attached.

## Discussion

Only one attribute of each type may be attached to each text view, with inner attributes taking precedence.

