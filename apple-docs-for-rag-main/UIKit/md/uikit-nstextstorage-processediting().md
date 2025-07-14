

- UIKit
- NSTextStorage
-  processEditing() 

Instance Method

# processEditing()

Cleans up changes to the text storage object and notifies its delegate and layout managers of changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func processEditing()
```

## Discussion

This method is automatically invoked in response to an edited(_:range:changeInLength:) message or an endEditing() message if edits were made within the scope of a beginEditing() block. You should never need to invoke it directly.

This method begins by posting an willProcessEditingNotification to the default notification center (which results in the delegate receiving a textStorage(_:willProcessEditing:range:changeInLength:) message). Then it fixes attributes. After this, it posts an didProcessEditingNotification to the default notification center (which results in the delegate receiving a textStorage(_:didProcessEditing:range:changeInLength:) message). Finally, it sends a textStorage(_:edited:range:changeInLength:invalidatedRange:) message to each of the receiver’s layout managers using the argument values provided.

## See Also

### Managing edits

func edited(NSTextStorage.EditActions, range: NSRange, changeInLength: Int)

Tracks changes made to the text storage object, allowing the text storage to record the full extent of changes.

