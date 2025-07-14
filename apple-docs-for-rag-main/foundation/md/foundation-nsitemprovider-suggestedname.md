

- Foundation
- NSItemProvider
-  suggestedName 

Instance Property

# suggestedName

The filename to use when writing the provided data to a file on disk.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
var suggestedName: String? { get set }
```

## Discussion

Setting this property is recommended when providing NSData or text data from an item provider.

## See Also

### Configuring the provider

var preferredPresentationSize: CGSize

The ideal presentation size of the item.

var preferredPresentationStyle: NSItemProvider.PreferredPresentationStyle

The preferred style for presenting the item provider’s data.

enum PreferredPresentationStyle

The presentation styles that determine how a view shows an item provider’s data.

var teamData: Data?

The collection of data an app uses to hold private team information during drag and drop.

