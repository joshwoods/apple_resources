

- Foundation
- NSItemProvider
-  preferredPresentationStyle 

Instance Property

# preferredPresentationStyle

The preferred style for presenting the item provider’s data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var preferredPresentationStyle: NSItemProvider.PreferredPresentationStyle { get set }
```

## Discussion

The default preferred presentation style is `unspecified`.

## See Also

### Configuring the provider

var preferredPresentationSize: CGSize

The ideal presentation size of the item.

enum PreferredPresentationStyle

The presentation styles that determine how a view shows an item provider’s data.

var suggestedName: String?

The filename to use when writing the provided data to a file on disk.

var teamData: Data?

The collection of data an app uses to hold private team information during drag and drop.

