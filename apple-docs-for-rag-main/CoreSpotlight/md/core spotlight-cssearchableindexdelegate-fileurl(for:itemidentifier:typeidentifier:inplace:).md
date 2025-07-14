

- Core Spotlight
- CSSearchableIndexDelegate
-  fileURL(for:itemIdentifier:typeIdentifier:inPlace:) 

Instance Method

# fileURL(for:itemIdentifier:typeIdentifier:inPlace:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
optional func fileURL(
    for searchableIndex: CSSearchableIndex,
    itemIdentifier: String,
    typeIdentifier: String,
    inPlace: Bool
) throws -> URL
```

## See Also

### Getting item-related details

func data(for: CSSearchableIndex, itemIdentifier: String, typeIdentifier: String) throws -> Data

