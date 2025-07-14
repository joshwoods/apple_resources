

- TVMLKit JS
- TVError
-  User Info Dictionary Keys 

API Collection

# User Info Dictionary Keys

Keys that exist in the user info dictionary.

## Topics

### Constants

NSLocalizedDesciptionKey

The corresponding value is a localized string representation of the error.

NSFilePathErrorKey

The corresponding value is a `String` object that contains the file path of the error.

NSStringEncodingErrorKey

The corresponding value is a `Number` object containing the `NSStringEncoding` value.

NSUnderlyingErrorKey

The corresponding value is an error that was encountered in an underlying implementation and caused the error that the receiver represents to occur.

NSURLErrorKey

The corresponding value is an NSURL object.

NSLocalizedFailureReasonErrorKey

The corresponding value is a localized string representation containing the reason for the failure that, if present, will be returned by localizedFailureReason.

NSLocalizedRecoverySuggestionErrorKey

The corresponding value is a string containing the localized recovery suggestion for the error. This string is suitable for displaying as the secondary message in an alert panel.

NSLocalizedRecoveryOptionsErrorKey

The corresponding value is an array containing the localized titles of buttons appropriate for displaying in an alert panel. The first string is the title of the right-most and default button, the second the one to the left, and so on. The recovery options should be appropriate for the recovery suggestion returned by `localizedRecoverySuggestion`.

NSRecoveryAttempterErrorKey

The corresponding value is an object that conforms to the NSErrorRecoveryAttempting informal protocol. The recovery attempter must be an object that can correctly interpret an index into the array returned by `recoveryAttempter`.

NSHelpAnchorErrorKey

The corresponding value is an NSString containing the localized help corresponding to the Help button. See helpAnchor for more information.

NSURLErrorFailingURLErrorKey

The corresponding value is an NSURL containing the URL which caused a load to fail. This key is only present in the NSURLErrorDomain.

NSURLErrorFailingURLStringErrorKey

The corresponding value is an NSString object for the URL which caused a load to fail. This key is only present in the NSURLErrorDomain.

NSURLErrorFailingURLPeerTrustErrorKey

The corresponding value is the SecTrust object representing the state of a failed SSL handshake. This key is only present in the NSURLErrorDomain.

