

- Foundation
- NSItemProvider
-  NSItemProvider.PreferredPresentationStyle 

Enumeration

# NSItemProvider.PreferredPresentationStyle

The presentation styles that determine how a view shows an item provider’s data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
enum PreferredPresentationStyle
```

## Topics

### Presentation Styles

case unspecified

A presentation style indicating that no preferred style is specified.

case inline

A presentation style indicating that the item provider data should be presented inline.

case attachment

A presentation style indicating that the item provider data should be presented as an attachment.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the provider

var preferredPresentationSize: CGSize

The ideal presentation size of the item.

var preferredPresentationStyle: NSItemProvider.PreferredPresentationStyle

The preferred style for presenting the item provider’s data.

var suggestedName: String?

The filename to use when writing the provided data to a file on disk.

var teamData: Data?

The collection of data an app uses to hold private team information during drag and drop.

