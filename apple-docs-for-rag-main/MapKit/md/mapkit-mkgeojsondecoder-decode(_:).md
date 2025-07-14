

- MapKit
- MKGeoJSONDecoder
-  decode(\_:) 

Instance Method

# decode(\_:)

Decodes the provided data into native MapKit types that a map can display.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func decode(_ data: Data) throws -> [any MKGeoJSONObject]
```

## Parameters 

`data`  

An NSData object that contains the JSON to decode.

## Return Value

An array of MKGeoJSONObject objects, or an error if the decoder encounters an issue.

