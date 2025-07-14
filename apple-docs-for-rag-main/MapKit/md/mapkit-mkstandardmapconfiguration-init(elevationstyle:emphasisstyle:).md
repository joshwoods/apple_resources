

- MapKit
- MKStandardMapConfiguration
-  init(elevationStyle:emphasisStyle:) 

Initializer

# init(elevationStyle:emphasisStyle:)

Creates a standard map configuration with the specified elevation and emphasis styles.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
convenience init(
    elevationStyle: MKMapConfiguration.ElevationStyle,
    emphasisStyle: MKStandardMapConfiguration.EmphasisStyle
)
```

## Parameters 

`elevationStyle`  

One of the MKMapConfiguration.ElevationStyle modes.

`emphasisStyle`  

One of the MKStandardMapConfiguration.EmphasisStyle styles.

## See Also

### Creating a standard map configuration

init()

Creates a new standard map configuration.

convenience init(elevationStyle: MKMapConfiguration.ElevationStyle)

Creates a new standard map configuration with the specified elevation style.

convenience init(emphasisStyle: MKStandardMapConfiguration.EmphasisStyle)

Creates a standard map configuration with the specified emphasis style.

enum ElevationStyle

Values that control the map’s elevation style.

enum EmphasisStyle

Values that control how the framework emphasizes map features.

