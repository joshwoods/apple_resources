

- File Provider
- NSFileProviderItemFields
-  contents 

Type Property

# contents

The item’s content.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
static var contents: NSFileProviderItemFields { get }
```

## Discussion

If the item is a directory, the content are the item’s children. If the item is a file, the content is the data saved on disk.

## See Also

### Specifying the Required Fields

static var filename: NSFileProviderItemFields

The item’s filename.

