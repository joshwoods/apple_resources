

- Quick Look
- QLPreviewController
-  delegate 

Instance Property

# delegate

The preview controller’s delegate object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any QLPreviewControllerDelegate)? { get set }
```

## Discussion

The delegate determines whether to open URLs that the user taps in a preview. See QLPreviewControllerDelegate to learn more.

## See Also

### Configuring a preview controller

var dataSource: (any QLPreviewControllerDataSource)?

The preview controller’s data source.

protocol QLPreviewControllerDataSource

The protocol that a data source for a preview controller needs to adopt to provide preview items to the controller.

protocol QLPreviewControllerDelegate

The protocol that a delegate of a preview controller needs to adopt to handle Quick Look previews.

