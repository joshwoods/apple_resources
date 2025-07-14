

- UIKit
- UIDocument
-  enableEditing() 

Instance Method

# enableEditing()

Enables editing when it’s safe again to make changes to a document.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func enableEditing()
```

## Discussion

Subclasses should override this method to allow the user to edit the document when it’s safe to do so. This method override should be paired with an override of disableEditing(). The default implementation of this method does nothing.

## See Also

### Disabling and enabling editing

func disableEditing()

Disables editing when it’s unsafe to make changes to a document.

