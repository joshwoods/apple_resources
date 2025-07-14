

- Foundation
- Locale
- Locale.Subdivision
-  init(\_:) 

Initializer

# init(\_:)

Creates a sudivision from a Unicode identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(_ identifier: String)
```

## Parameters 

`identifier`  

The subdivision’s identifier.

## See Also

### Creating a subdivision

static func subdivision(for: Locale.Region) -> Locale.Subdivision

Returns the subdivision representing the given region as a whole.

