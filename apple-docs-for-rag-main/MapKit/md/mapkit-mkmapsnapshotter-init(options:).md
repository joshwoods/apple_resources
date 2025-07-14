

- MapKit
- MKMapSnapshotter
-  init(options:) 

Initializer

# init(options:)

Creates and returns a snapshotter object based on the specified options.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
init(options: MKMapSnapshotter.Options)
```

## Parameters 

`options`  

The options to use when capturing the map imagery. See MKMapSnapshotter.Options. This parameter may not be `nil`.

## Return Value

An initialized snapshotter object.

## See Also

### Creating a snapshotter object

class Options

The options the snapshotter initializer uses to create a snapshotter to capture map-based imagery.

