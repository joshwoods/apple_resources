

- Assets Library
-  ALAssetsLibraryAccessGloballyDeniedError 

Global Variable

# ALAssetsLibraryAccessGloballyDeniedError

Access to the library was denied globally.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+

``` source
var ALAssetsLibraryAccessGloballyDeniedError: Int { get }
```

## Discussion

This error may be returned in the ALAssetsLibraryAccessFailureBlock block for enumerateGroups(withTypes:using:failureBlock:) and asset(for:resultBlock:failureBlock:).

## See Also

### Constants

var ALAssetsLibraryUnknownError: Int

The reason for the error is unknown.

var ALAssetsLibraryWriteFailedError: Int

The attempt to write data failed.

var ALAssetsLibraryWriteBusyError: Int

Writing was already busy when the attempt to write was made.

var ALAssetsLibraryWriteInvalidDataError: Int

The data was invalid.

var ALAssetsLibraryWriteIncompatibleDataError: Int

The data contained incompatible data.

var ALAssetsLibraryWriteDataEncodingError: Int

The data contained data with the wrong encoding.

var ALAssetsLibraryWriteDiskSpaceError: Int

There was not enough space on the disk to write the data.

var ALAssetsLibraryDataUnavailableError: Int

The data was not available.

var ALAssetsLibraryAccessUserDeniedError: Int

The user denied access to the library.

