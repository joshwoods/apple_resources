

- UIKit
- NSTextAttachmentViewProvider
-  loadView() 

Instance Method

# loadView()

Draws the custom view hierarchy that text attachment view subclasses implement.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func loadView()
```

## Discussion

Use this method to create a custom view hierarchy. Don’t call this method directly, the framework calls it at the appropriate time.

