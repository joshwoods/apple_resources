

- MediaExtension
- MEFormatReader
-  loadTrackReaders(completionHandler:) 

Instance Method

# loadTrackReaders(completionHandler:)

Loads the array of track readers that represent the tracks in the media asset.

macOS 14.0+

``` source
func loadTrackReaders(completionHandler: @escaping ([any METrackReader]?, (any Error)?) -> Void)
```

``` source
var trackReaders: [any METrackReader] { get async throws }
```

**Required**

## Parameters 

`completionHandler`  

The completion block to execute when the load operation finishes.

## See Also

### Reading and parsing media assets

func loadFileInfo(completionHandler: (MEFileInfo?, (any Error)?) -> Void)

Loads the file info object with the properties of the media asset.

**Required**

func loadMetadata(completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads the array of metadata items from the media asset.

**Required**

func parseAdditionalFragments(completionHandler: (MEFormatReaderParseAdditionalFragmentsStatus, (any Error)?) -> Void)

Incorporates additional fragments that the file received after the last time the format reader parsed it.

struct MEFormatReaderParseAdditionalFragmentsStatus

Informational status flags that the format reader returns after parsing additional fragments.

