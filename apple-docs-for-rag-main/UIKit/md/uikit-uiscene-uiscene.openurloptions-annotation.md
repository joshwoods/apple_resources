

- UIKit
- UIScene
- UIScene.OpenURLOptions
-  annotation 

Instance Property

# annotation

A property-list object that contains the annotation data provided by a document interaction controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var annotation: Any? { get }
```

## Discussion

This property contains the data that the originating app placed in the annotation property of its UIDocumentInteractionController. The root object is always an NSDictionary object. The contents of that dictionary may be any other property list types, including NSDictionary, NSArray, NSData, NSString, NSNumber, or NSDate objects.

## See Also

### Specifying the URL details

var sourceApplication: String?

The bundle ID of the app that originated the request.

var eventAttribution: UIEventAttribution?

An event attribution associated with the URL to open.

