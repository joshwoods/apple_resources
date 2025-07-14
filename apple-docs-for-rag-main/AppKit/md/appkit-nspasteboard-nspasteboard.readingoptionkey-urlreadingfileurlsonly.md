

- AppKit
- NSPasteboard
- NSPasteboard.ReadingOptionKey
-  urlReadingFileURLsOnly 

Type Property

# urlReadingFileURLsOnly

Option for reading URLs to restrict the results to file URLs only.

macOS 10.6+

``` source
static let urlReadingFileURLsOnly: NSPasteboard.ReadingOptionKey
```

## Discussion

The value for this key is an `NSNumber` object with a boolean value.

## See Also

### Type Properties

static let urlReadingContentsConformToTypes: NSPasteboard.ReadingOptionKey

Option for reading URLs to restrict the results to URLs with contents that conform to any of the provided UTI types.

