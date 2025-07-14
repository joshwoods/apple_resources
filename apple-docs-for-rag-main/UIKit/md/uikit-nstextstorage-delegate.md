

- UIKit
- NSTextStorage
-  delegate 

Instance Property

# delegate

The delegate for the text storage object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
weak var delegate: (any NSTextStorageDelegate)? { get set }
```

## Discussion

Use a delegate object to monitor edits occurring to the text contents. Your delegate object must conform to the NSTextStorageDelegate protocol.

## See Also

### Processing the editing actions

protocol NSTextStorageDelegate

The optional methods that delegates of text storage objects implement to handle text-edit processing.

