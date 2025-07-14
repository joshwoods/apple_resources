

- Foundation
- Errors and Exceptions
- NSError
-  NSError Codes 

API Collection

# NSError Codes

Error codes in the Cocoa error domain.

## Overview

The constants in this enumeration are NSError code numbers in the Cocoa error domain (NSCocoaErrorDomain). Other frameworks, most notably the Application Kit, provide their own NSCocoaErrorDomain error codes.

The enumeration constants beginning with `NSFile` indicate file-system errors or errors related to file I/O operations. Use the key NSFilePathErrorKey or the NSURLErrorKey (whichever is appropriate) to access the file-system path or URL in the userInfo dictionary of the NSError object.

## Topics

### Bundle Errors

var NSBundleErrorMinimum: Int

The start of the range of error codes reserved for bundle errors.

var NSBundleErrorMaximum: Int

The end of the range of error codes reserved for bundle errors.

var NSBundleOnDemandResourceExceededMaximumSizeError: Int

The application exceeded the amount of on-demand resources content in use at one time.

var NSBundleOnDemandResourceInvalidTagError: Int

The application specified a tag that the system couldn’t find in the application tag manifest.

var NSBundleOnDemandResourceOutOfSpaceError: Int

Insufficient space available to download the requested on-demand resources.

### Cancellation

var NSUserCancelledError: Int

The user canceled the operation (for example, by pressing Command-period).

### Cloud-Sharing Errors

var NSCloudSharingErrorMinimum: Int

The start of the range of error codes reserved for cloud-sharing errors.

var NSCloudSharingErrorMaximum: Int

The end of the range of error codes reserved for cloud-sharing errors.

var NSCloudSharingConflictError: Int

A conflict occurred during an attempt to save changes.

var NSCloudSharingNetworkFailureError: Int

Sharing failed due to a network failure.

var NSCloudSharingNoPermissionError: Int

The current user doesn’t have permission to perform the requested actions.

var NSCloudSharingOtherError: Int

An otherwise unspecified cloud-sharing error occurred.

var NSCloudSharingQuotaExceededError: Int

The user doesn’t have enough storage space available to share the requested items.

var NSCloudSharingTooManyParticipantsError: Int

Additional participants couldn’t be added to the share, because the limit was reached.

### Coder Errors

var NSCoderErrorMinimum: Int

The start of the range of error codes reserved for coder errors.

var NSCoderErrorMaximum: Int

The end of the range of error codes reserved for coder errors.

var NSCoderValueNotFoundError: Int

The requested data wasn’t found.

var NSCoderReadCorruptError: Int

Decoding failed due to corrupt data.

### Executable Errors

var NSExecutableErrorMinimum: Int

The beginning of the range of error codes reserved for errors related to executable files.

var NSExecutableErrorMaximum: Int

The end of the range of error codes reserved for errors related to executable files.

var NSExecutableArchitectureMismatchError: Int

The executable doesn’t provide an architecture compatible with the current process.

var NSExecutableLinkError: Int

The executable failed due to linking issues.

var NSExecutableLoadError: Int

Executable cannot be loaded for an otherwise-unspecified reason.

var NSExecutableNotLoadableError: Int

The executable type isn’t loadable in the current process.

var NSExecutableRuntimeMismatchError: Int

The executable has Objective-C runtime information that’s incompatible with the current process.

### Formatting Errors

var NSFormattingErrorMinimum: Int

The start of the range of error codes reserved for formatting errors.

var NSFormattingErrorMaximum: Int

The end of the range of error codes reserved for formatting errors.

var NSFormattingError: Int

A formatter couldn’t generate a string for an object, or parse a string into an object.

### File Errors

var NSFileErrorMinimum: Int

The start of the range of error codes reserved for file errors.

var NSFileErrorMaximum: Int

The end of the range of error codes reserved for file errors.

var NSFileLockingError: Int

The file could not be locked.

var NSFileManagerUnmountBusyError: Int

The volume couldn’t be unmounted because it’s in use.

var NSFileManagerUnmountUnknownError: Int

The volume couldn’t be unmounted, for unknown reasons.

var NSFileNoSuchFileError: Int

A filesystem operation was attempted on a non-existent file.

### File Reading Errors

var NSFileReadCorruptFileError: Int

Could not read because of a corrupted file, bad format, or similar reason.

var NSFileReadInapplicableStringEncodingError: Int

Could not read because the string encoding wasn’t applicable.

var NSFileReadInvalidFileNameError: Int

Could not read because of an invalid file name.

var NSFileReadNoPermissionError: Int

Could not read because of a permission problem.

var NSFileReadNoSuchFileError: Int

Could not read because no such file was found.

var NSFileReadTooLargeError: Int

Could not read because the specified file was too large.

var NSFileReadUnknownError: Int

Could not read, for unknown reasons.

var NSFileReadUnknownStringEncodingError: Int

Could not read because the string coding of the file couldn’t be determined.

var NSFileReadUnsupportedSchemeError: Int

Could not read because the specified URL scheme is unsupported.

### File Writing Errors

var NSFileWriteFileExistsError: Int

Could not perform an operation because the destination file already exists.

var NSFileWriteInapplicableStringEncodingError: Int

Could not write because the string encoding was not applicable.

var NSFileWriteInvalidFileNameError: Int

Could not write because of an invalid file name.

var NSFileWriteNoPermissionError: Int

Could not write because of a permission problem.

var NSFileWriteOutOfSpaceError: Int

Could not write because of a lack of disk space.

var NSFileWriteUnknownError: Int

Could not write, for unknown reasons.

var NSFileWriteUnsupportedSchemeError: Int

Could not write because the specified URL scheme is unsupported.

var NSFileWriteVolumeReadOnlyError: Int

Could not write because the volume is read-only.

### iCloud File Errors

var NSUbiquitousFileErrorMinimum: Int

The minimum error code value that represents an iCloud error.

var NSUbiquitousFileErrorMaximum: Int

The maximum error code value that represents an iCloud error.

var NSUbiquitousFileNotUploadedDueToQuotaError: Int

The item could not be uploaded to iCloud because it would make the account go over its quota.

var NSUbiquitousFileUbiquityServerNotAvailable: Int

A failure to connect to the iCloud servers.

var NSUbiquitousFileUnavailableError: Int

The item has not been uploaded to iCloud by another device yet.

### Property List Errors

var NSPropertyListErrorMinimum: Int

The start of the range of error codes reserved for property list errors.

var NSPropertyListErrorMaximum: Int

The end of the range of error codes reserved for property list errors.

var NSPropertyListReadCorruptError: Int

Parsing of the property list failed.

var NSPropertyListReadStreamError: Int

Reading of the property list failed.

var NSPropertyListReadUnknownVersionError: Int

The version number of the property list cannot be determined.

var NSPropertyListWriteInvalidError: Int

Writing failed because of an invalid property list object, or an invalid property list type was specified.

var NSPropertyListWriteStreamError: Int

Writing to the property list failed.

### User Activity Errors

var NSUserActivityErrorMinimum: Int

The start of the range of error codes reserved for user activity errors.

var NSUserActivityErrorMaximum: Int

The end of the range of error codes reserved for user activity errors.

var NSUserActivityConnectionUnavailableError: Int

The user activity couldn’t be continued because a required connection wasn’t available.

var NSUserActivityHandoffFailedError: Int

The data for the user activity wasn’t available.

var NSUserActivityHandoffUserInfoTooLargeError: Int

The user info dictionary was too large to receive.

var NSUserActivityRemoteApplicationTimedOutError: Int

The remote application failed to send data within the specified time.

### Validation Errors

var NSValidationErrorMinimum: Int

The start of the range of error codes reserved for validation errors.

var NSValidationErrorMaximum: Int

The end of the range of error codes reserved for validation errors.

### XPC Errors

var NSXPCConnectionErrorMinimum: Int

The lower bounds of XPC connection error code values.

var NSXPCConnectionErrorMaximum: Int

The upper bounds of XPC connection error code values.

var NSXPCConnectionInterrupted: Int

The XPC connection was interrupted.

var NSXPCConnectionInvalid: Int

The XPC connection was invalid.

var NSXPCConnectionReplyInvalid: Int

The XPC connection reply was invalid.

### URL Errors

var NSURLErrorAppTransportSecurityRequiresSecureConnection: Int

App Transport Security disallowed a connection because there is no secure network connection.

var NSURLErrorBackgroundSessionInUseByAnotherProcess: Int

An app or app extension attempted to connect to a background session that is already connected to a process.

var NSURLErrorBackgroundSessionRequiresSharedContainer: Int

The shared container identifier of the URL session configuration is needed but hasn’t been set.

var NSURLErrorBackgroundSessionWasDisconnected: Int

The app is suspended or exits while a background data task is processing.

var NSURLErrorBadServerResponse: Int

The URL Loading System received bad data from the server.

var NSURLErrorBadURL: Int

A malformed URL prevented a URL request from being initiated.

var NSURLErrorCallIsActive: Int

A connection was attempted while a phone call was active on a network that doesn’t support simultaneous phone and data communication, such as EDGE or GPRS.

var NSURLErrorCancelled: Int

An asynchronous load has been canceled.

var NSURLErrorCannotCloseFile: Int

A download task couldn’t close the downloaded file on disk.

var NSURLErrorCannotConnectToHost: Int

An attempt to connect to a host failed.

var NSURLErrorCannotCreateFile: Int

A download task couldn’t create the downloaded file on disk because of an I/O failure.

var NSURLErrorCannotDecodeContentData: Int

Content data received during a connection request had an unknown content encoding.

var NSURLErrorCannotDecodeRawData: Int

Content data received during a connection request couldn’t be decoded for a known content encoding.

var NSURLErrorCannotFindHost: Int

The host name for a URL couldn’t be resolved.

var NSURLErrorCannotLoadFromNetwork: Int

A specific request to load an item only from the cache couldn’t be satisfied.

var NSURLErrorCannotMoveFile: Int

A downloaded file on disk couldn’t be moved.

var NSURLErrorCannotOpenFile: Int

A downloaded file on disk couldn’t be opened.

var NSURLErrorCannotParseResponse: Int

A response to a connection request couldn’t be parsed.

var NSURLErrorCannotRemoveFile: Int

A downloaded file couldn’t be removed from disk.

var NSURLErrorCannotWriteToFile: Int

A download task couldn’t write the file to disk.

var NSURLErrorClientCertificateRejected: Int

A server certificate was rejected.

var NSURLErrorClientCertificateRequired: Int

A client certificate was required to authenticate an SSL connection during a connection request.

var NSURLErrorDNSLookupFailed: Int

The host address couldn’t be found via DNS lookup.

var NSURLErrorDataLengthExceedsMaximum: Int

The length of the resource data exceeded the maximum allowed.

var NSURLErrorDataNotAllowed: Int

The cellular network disallowed a connection.

var NSURLErrorDownloadDecodingFailedMidStream: Int

A download task failed to decode an encoded file during the download.

var NSURLErrorDownloadDecodingFailedToComplete: Int

A download task failed to decode an encoded file after downloading.

var NSURLErrorFileDoesNotExist: Int

The specified file doesn’t exist.

var NSURLErrorFileIsDirectory: Int

A request for an FTP file resulted in the server responding that the file is not a plain file, but a directory.

var NSURLErrorFileOutsideSafeArea: Int

An internal file operation failed.

var NSURLErrorHTTPTooManyRedirects: Int

A redirect loop was detected or the threshold for number of allowable redirects was exceeded (currently 16).

var NSURLErrorInternationalRoamingOff: Int

The attempted connection required activating a data context while roaming, but international roaming is disabled.

var NSURLErrorNetworkConnectionLost: Int

A client or server connection was severed in the middle of an in-progress load.

var NSURLErrorNoPermissionsToReadFile: Int

A resource couldn’t be read because of insufficient permissions.

var NSURLErrorNotConnectedToInternet: Int

A network resource was requested, but an internet connection has not been established and can’t be established automatically.

var NSURLErrorRedirectToNonExistentLocation: Int

A redirect was specified by way of server response code, but the server didn’t accompany this code with a redirect URL.

var NSURLErrorRequestBodyStreamExhausted: Int

A body stream was needed but the client did not provide one.

var NSURLErrorResourceUnavailable: Int

A requested resource couldn’t be retrieved.

var NSURLErrorSecureConnectionFailed: Int

An attempt to establish a secure connection failed for reasons that can’t be expressed more specifically.

var NSURLErrorServerCertificateHasBadDate: Int

A server certificate is expired, or is not yet valid.

var NSURLErrorServerCertificateHasUnknownRoot: Int

A server certificate wasn’t signed by any root server.

var NSURLErrorServerCertificateNotYetValid: Int

A server certificate isn’t valid yet.

var NSURLErrorServerCertificateUntrusted: Int

A server certificate was signed by a root server that isn’t trusted.

var NSURLErrorTimedOut: Int

An asynchronous operation timed out.

var NSURLErrorUnknown: Int

The URL Loading System encountered an error that it can’t interpret.

var NSURLErrorUnsupportedURL: Int

A properly formed URL couldn’t be handled by the framework.

var NSURLErrorUserAuthenticationRequired: Int

Authentication was required to access a resource.

var NSURLErrorUserCancelledAuthentication: Int

An asynchronous request for authentication has been canceled by the user.

var NSURLErrorZeroByteResource: Int

A server reported that a URL has a non-zero content length, but terminated the network connection gracefully without sending any data.

### Miscellaneous Errors

var NSFeatureUnsupportedError: Int

The feature isn’t supported, because the file system lacks the feature, or required libraries are missing, or other similar reasons.

var NSKeyValueValidationError: Int

A key-value coding validation error.

## See Also

### Error Codes

struct CocoaError

Describes errors within the Cocoa error domain.

struct MachError

Describes an error in the Mach error domain.

struct POSIXError

Describes an error in the POSIX error domain.

