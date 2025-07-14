

- BrowserEngineKit
- Text interaction
-  Supporting extended text interactions 

Article

# Supporting extended text interactions

Share content, add replacement shortcuts, and perform other rich actions in browser text views.

## Overview

When your browser’s text view conforms to the BETextInput protocol, it automatically also conforms to BEResponderEditActions. This protocol adds a collection of optional action methods your text view can implement to support extended text interactions.

To get the operating system’s standard behavior for an interaction, add a BETextInteraction to your custom view’s textInputView, and call the interaction’s methods in response to `BEResponderEditActions`.

Additionally, implement canPerformAction(_:withSender:), to return `true` in situations where the interaction is available, but `false` otherwise.

For example, to share the selected text using the standard share sheet:

```
class MyBrowserTextView: UIView, BETextInput, BEResponderEditActions {
  func canPerformAction(_ action: Selector, withSender sender: Any?) -> Bool {
   if (action == #selector(share(_:))) {
     return self.canShareSelection
   }
  }

  func share(_ sender: Any?) {
    self.textInteraction.shareText(self.selectedText, from:self.selectionRect)
  }
}
```

## See Also

### Custom text views

Integrating custom browser text views with UIKit

Process keyboard interactions asynchronously in your iOS browser app’s text view.

protocol BETextInput

A protocol to which text views conform to asynchronously integrate with the text system.

protocol BETextInputDelegate

A delegate protocol that a browser text view uses to notify the text system of changes.

