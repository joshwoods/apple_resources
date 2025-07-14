

- UIKit
- UIScene
- UIScene.OpenURLOptions
-  eventAttribution 

Instance Property

# eventAttribution

An event attribution associated with the URL to open.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
var eventAttribution: UIEventAttribution? { get }
```

## Discussion

For more information about event attribution data, see UIEventAttribution.

## See Also

### Specifying the URL details

var sourceApplication: String?

The bundle ID of the app that originated the request.

var annotation: Any?

A property-list object that contains the annotation data provided by a document interaction controller.

