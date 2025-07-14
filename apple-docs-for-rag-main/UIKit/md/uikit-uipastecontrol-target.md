

- UIKit
- UIPasteControl
-  target 

Instance Property

# target

The UI control that receives pasted content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
weak var target: (any UIPasteConfigurationSupporting)? { get set }
```

## Discussion

For example, you can assign this property a reference to a UITextView.

