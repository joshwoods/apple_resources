

- PencilKit
- PKToolPicker
-  maximumSupportedContentVersion 

Instance Property

# maximumSupportedContentVersion

The maximum version of PencilKit to support.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
var maximumSupportedContentVersion: PKContentVersion { get set }
```

## Mentioned in 

Supporting backward compatibility for ink types

## Discussion

The default value is latest.

If you set this property to a value less than latest, the tool picker limits the tools that are available so they’re compatible with the version of PencilKit you specify.

If you set this property, also set maximumSupportedContentVersion on the PKCanvasView you use.

