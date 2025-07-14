

- UIKit
- UITextInput
-  isEditable 

Instance Property

# isEditable

A Boolean value that indicates whether the text view contains editable text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
optional var isEditable: Bool { get }
```

## Discussion

Text views are normally editable, and the default value of this property is true if you don’t provide an implementation. When implementing a custom text view, you might implement this property and return false to prevent outside agents from modifying the content of your view. For example, you might disable editing to prevent the system’s writing tools panel from pasting content into your view.

