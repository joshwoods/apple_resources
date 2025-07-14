

- MapKit
- MKStandardMapConfiguration
-  MKStandardMapConfiguration.EmphasisStyle 

Enumeration

# MKStandardMapConfiguration.EmphasisStyle

Values that control how the framework emphasizes map features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum EmphasisStyle
```

## Topics

### Controlling the map’s emphasis

case `default`

The default level of emphasis.

case muted

The muted level of emphasis.

case `default`

The default level of emphasis.

case muted

The muted level of emphasis.

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

### Creating a standard map configuration

init()

Creates a new standard map configuration.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle)

Creates a new standard map configuration with the specified elevation style.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle, emphasisStyle: MKStandardMapConfiguration.EmphasisStyle)

Creates a standard map configuration with the specified elevation and emphasis styles.

convenience init(emphasisStyle: MKStandardMapConfiguration.EmphasisStyle)

Creates a standard map configuration with the specified emphasis style.

enum ElevationStyle

Values that control the map’s elevation style.

