

- Quick Look
- QLPreviewController
-  dataSource 

Instance Property

# dataSource

The preview controller’s data source.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var dataSource: (any QLPreviewControllerDataSource)? { get set }
```

## Discussion

To use a Quick Look preview controller, you need to implement a data source. The data source is responsible for providing items for display by the controller, and for telling it how many items to include in the preview navigation list. To learn more about implementing a data source, see QLPreviewControllerDataSource.

## See Also

### Configuring a preview controller

protocol QLPreviewControllerDataSource

The protocol that a data source for a preview controller needs to adopt to provide preview items to the controller.

var delegate: (any QLPreviewControllerDelegate)?

The preview controller’s delegate object.

protocol QLPreviewControllerDelegate

The protocol that a delegate of a preview controller needs to adopt to handle Quick Look previews.

