

- Foundation
- Locale
- Locale.Subdivision
-  subdivision(for:) 

Type Method

# subdivision(for:)

Returns the subdivision representing the given region as a whole.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func subdivision(for region: Locale.Region) -> Locale.Subdivision
```

## Parameters 

`region`  

A region to represent as a subdivision.

## Return Value

A subdivision that represents the entire region.

## Discussion

For example, this method returns a subdivision with the `uszzzz` identifier for the entire US region.

## See Also

### Creating a subdivision

init(String)

Creates a sudivision from a Unicode identifier.

