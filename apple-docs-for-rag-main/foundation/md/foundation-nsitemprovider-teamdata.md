

- Foundation
- NSItemProvider
-  teamData 

Instance Property

# teamData

The collection of data an app uses to hold private team information during drag and drop.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var teamData: Data? { get set }
```

## See Also

### Configuring the provider

var preferredPresentationSize: CGSize

The ideal presentation size of the item.

var preferredPresentationStyle: NSItemProvider.PreferredPresentationStyle

The preferred style for presenting the item provider’s data.

enum PreferredPresentationStyle

The presentation styles that determine how a view shows an item provider’s data.

var suggestedName: String?

The filename to use when writing the provided data to a file on disk.

