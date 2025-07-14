

- App Intents
- IntentFile
-  filename 

Instance Property

# filename

The human-readable name of the file, which will be displayed to the user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var filename: String { get }
```

## See Also

### Getting the file information

var fileURL: URL?

URL to the file on disk, if any. If the file isn’t stored on disk, access the contents using the `data` property.

var type: UTType?

The uniform type identifier of the file. (i.e. “public.json”, “public.png”, or any custom type) More information about uniform type identifiers can be found in \

var data: Data

The contents of the file. If the file was created with a URL, accessing this property will memory map the file contents.

var removedOnCompletion: Bool

Indicates whether the file should be automatically deleted from disk when the Shortcut is done running. `false` by default.

