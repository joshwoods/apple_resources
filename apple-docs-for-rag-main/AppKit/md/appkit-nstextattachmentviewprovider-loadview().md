

- AppKit
- NSTextAttachmentViewProvider
-  loadView() 

Instance Method

# loadView()

Draws the custom view hierarchy that text attachment view subclasses implement.

macOS 12.0+

``` source
func loadView()
```

## Discussion

Use this method to create a custom view hierarchy. Don’t call this method directly, the framework calls it at the appropriate time.

