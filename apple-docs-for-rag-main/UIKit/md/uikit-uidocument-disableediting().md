

- UIKit
- UIDocument
-  disableEditing() 

Instance Method

# disableEditing()

Disables editing when it’s unsafe to make changes to a document.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func disableEditing()
```

## Discussion

Subclasses should override this method to prevent the user from editing the document when it’s unsafe to do so, such as during a save-and-close or revert operation. When editing is safe again, UIKit class calls enableEditing(). The default implementation of this method does nothing.

## See Also

### Disabling and enabling editing

func enableEditing()

Enables editing when it’s safe again to make changes to a document.

