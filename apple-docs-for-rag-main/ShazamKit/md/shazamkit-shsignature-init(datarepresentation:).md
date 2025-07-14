

- ShazamKit
- SHSignature
-  init(dataRepresentation:) 

Initializer

# init(dataRepresentation:)

Creates a signature object from raw data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(dataRepresentation: Data) throws
```

## Parameters 

`dataRepresentation`  

The raw data for the signature.

## Return Value

A signature if the raw data is a valid signature; otherwise, `nil`.

