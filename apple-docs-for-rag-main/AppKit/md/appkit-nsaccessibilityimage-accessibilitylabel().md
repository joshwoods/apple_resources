

- AppKit
- NSAccessibilityImage
-  accessibilityLabel() 

Instance Method

# accessibilityLabel()

Returns a short description of the image’s label.

macOS

``` source
func accessibilityLabel() -> String?
```

**Required**

## Return Value

The description of the images label.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityLabel property.

Do not include the accessibility element’s type in the label (for example, write `Play`, not `Play button`.). If possible, use a single word. To help ensure that accessibility clients such as VoiceOver read the label with the correct intonation, start this label with a capital letter. Do not put a period at the end. Always localize the label.

