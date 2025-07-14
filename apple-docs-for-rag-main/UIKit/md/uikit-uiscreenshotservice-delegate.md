

- UIKit
- UIScreenshotService
-  delegate 

Instance Property

# delegate

The custom object you use to provide PDF data for a screenshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+

``` source
@MainActor
weak var delegate: (any UIScreenshotServiceDelegate)? { get set }
```

## Discussion

Assign an object to this property early in the life cycle of your window scene. The object must conform to the UIScreenshotServiceDelegate protocol.

## See Also

### Responding to screenshot requests

protocol UIScreenshotServiceDelegate

Methods you use to generate PDF data that accompanies a user-requested screenshot.

