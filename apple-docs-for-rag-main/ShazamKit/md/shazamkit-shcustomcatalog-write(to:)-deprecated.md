

- ShazamKit
- SHCustomCatalog
-  write(to:) Deprecated

Instance Method

# write(to:)

Saves the custom catalog to a local file.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
func write(to destinationURL: URL) throws
```

Deprecated

Use dataRepresentation

## Parameters 

`destinationURL`  

A URL for the saved custom catalog file.

## Discussion

If `destinationURL` is a directory, the system creates a `Signatures.shazamcatalog` file.

## See Also

### Loading and saving a custom catalog

func add(from: URL) throws

Loads a saved custom catalog from a file.

