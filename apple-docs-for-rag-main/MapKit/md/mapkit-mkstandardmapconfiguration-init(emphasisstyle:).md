

- MapKit
- MKStandardMapConfiguration
-  init(emphasisStyle:) 

Initializer

# init(emphasisStyle:)

Creates a standard map configuration with the specified emphasis style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
convenience init(emphasisStyle: MKStandardMapConfiguration.EmphasisStyle)
```

## Parameters 

`emphasisStyle`  

One of the MKStandardMapConfiguration.EmphasisStyle styles.

## See Also

### Creating a standard map configuration

init()

Creates a new standard map configuration.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle)

Creates a new standard map configuration with the specified elevation style.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle, emphasisStyle: MKStandardMapConfiguration.EmphasisStyle)

Creates a standard map configuration with the specified elevation and emphasis styles.

enum ElevationStyle

Values that control the map’s elevation style.

enum EmphasisStyle

Values that control how the framework emphasizes map features.

