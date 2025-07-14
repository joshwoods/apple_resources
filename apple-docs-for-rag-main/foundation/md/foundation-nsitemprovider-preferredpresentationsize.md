

- Foundation
- NSItemProvider
-  preferredPresentationSize 

Instance Property

# preferredPresentationSize

The ideal presentation size of the item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

**macOS**

``` source
var preferredPresentationSize: NSSize { get }
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
var preferredPresentationSize: CGSize { get set }
```

## Discussion

When displaying the item, the value in this property represents the ideal size at which to display the item. The size in this property may differ from the size in the sourceFrame rectangle. For images, video, and other content with a natural size, the item automatically derives the size from that content. If the value in this property is NSZeroSize, use the size specified in the sourceFrame rectangle.

## See Also

### Configuring the provider

var preferredPresentationStyle: NSItemProvider.PreferredPresentationStyle

The preferred style for presenting the item provider’s data.

enum PreferredPresentationStyle

The presentation styles that determine how a view shows an item provider’s data.

var suggestedName: String?

The filename to use when writing the provided data to a file on disk.

var teamData: Data?

The collection of data an app uses to hold private team information during drag and drop.

