

- MediaExtension
- MEFormatReader
-  parseAdditionalFragments(completionHandler:) 

Instance Method

# parseAdditionalFragments(completionHandler:)

Incorporates additional fragments that the file received after the last time the format reader parsed it.

macOS 14.0+

``` source
optional func parseAdditionalFragments(completionHandler: @escaping (MEFormatReaderParseAdditionalFragmentsStatus, (any Error)?) -> Void)
```

``` source
optional func parseAdditionalFragments() async throws -> MEFormatReaderParseAdditionalFragmentsStatus
```

## Parameters 

`completionHandler`  

The completion block to execute when the parse operation finishes.

## Discussion

This method additional fragments of the media asset if they exist. Media asset formats that don’t support incremental fragments don’t need implement this method. Create the MEFormatReader object with the MEFormatReaderInstantiationOptions property allowIncrementalFragmentParsing set to true. This method does nothing if the value for MEFileInfo.FragmentsStatus is MEFileInfo.FragmentsStatus.containsFragments. Once this method returns an error, additional calls fail.

## See Also

### Reading and parsing media assets

func loadFileInfo(completionHandler: (MEFileInfo?, (any Error)?) -> Void)

Loads the file info object with the properties of the media asset.

**Required**

func loadMetadata(completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads the array of metadata items from the media asset.

**Required**

func loadTrackReaders(completionHandler: ([any METrackReader]?, (any Error)?) -> Void)

Loads the array of track readers that represent the tracks in the media asset.

**Required**

struct MEFormatReaderParseAdditionalFragmentsStatus

Informational status flags that the format reader returns after parsing additional fragments.

