

- AppKit
- NSPasteboard
- NSPasteboard.ReadingOptionKey
-  urlReadingContentsConformToTypes 

Type Property

# urlReadingContentsConformToTypes

Option for reading URLs to restrict the results to URLs with contents that conform to any of the provided UTI types.

macOS 10.6+

``` source
static let urlReadingContentsConformToTypes: NSPasteboard.ReadingOptionKey
```

## Discussion

If the content type of a URL cannot be determined, it will not be considered to match. The value for this key is an array of UTI type strings.

## See Also

### Type Properties

static let urlReadingFileURLsOnly: NSPasteboard.ReadingOptionKey

Option for reading URLs to restrict the results to file URLs only.

