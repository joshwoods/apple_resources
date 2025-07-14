

- Foundation
-  NSExceptionName 

Structure

# NSExceptionName

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSExceptionName
```

## Topics

### Type Properties

static let characterConversionException: NSExceptionName

`NSString` raises an `NSCharacterConversionException` if a string cannot be represented in a file-system or string encoding.

static let decimalNumberDivideByZeroException: NSExceptionName

The exception raised on divide by zero.

static let decimalNumberExactnessException: NSExceptionName

The exception raised if there is an exactness error.

static let decimalNumberOverflowException: NSExceptionName

The exception raised on overflow.

static let decimalNumberUnderflowException: NSExceptionName

The exception raised on underflow.

static let destinationInvalidException: NSExceptionName

Name of an exception that occurs when an internal assertion fails and implies an unexpected condition within the distributed objects.

static let fileHandleOperationException: NSExceptionName

Raised by `NSFileHandle` if attempts to determine file-handle type fail or if attempts to read from a file or channel fail.

static let genericException: NSExceptionName

A generic name for an exception.

static let internalInconsistencyException: NSExceptionName

Name of an exception that occurs when an internal assertion fails and implies an unexpected condition within the called code.

static let invalidArchiveOperationException: NSExceptionName

The name of the exception raised by `NSKeyedArchiver` if there is a problem creating an archive.

static let invalidArgumentException: NSExceptionName

Name of an exception that occurs when you pass an invalid argument to a method, such as a `nil` pointer where a non-`nil` object is required.

static let invalidReceivePortException: NSExceptionName

Name of an exception that occurs when the receive port of an `NSConnection` has become invalid.

static let invalidSendPortException: NSExceptionName

Name of an exception that occurs when the send port of an `NSConnection` has become invalid.

static let invalidUnarchiveOperationException: NSExceptionName

The name of the exception raised by `NSKeyedArchiver` if there is a problem extracting an archive.

static let invocationOperationCancelledException: NSExceptionName

The name of the exception raised if the result method is called after the operation was cancelled.

static let invocationOperationVoidResultException: NSExceptionName

The name of the exception raised if the result method is called for an invocation method with a `void` return type.

static let mallocException: NSExceptionName

Obsolete; not currently used.

static let objectInaccessibleException: NSExceptionName

Name of an exception that occurs when a remote object is accessed from a thread that should not access it.

static let objectNotAvailableException: NSExceptionName

Name of an exception that occurs when the remote side of the `NSConnection` refused to send the message to the object because the object has never been vended.

static let oldStyleException: NSExceptionName

No longer used.

static let parseErrorException: NSExceptionName

`NSString` raises an `NSParseErrorException` if a string cannot be parsed as a property list.

static let portReceiveException: NSExceptionName

Generic error occurred on receive.

static let portSendException: NSExceptionName

Generic error occurred on send.

static let portTimeoutException: NSExceptionName

Name of an exception that occurs when a timeout set on a port expires during a send or receive operation.

static let rangeException: NSExceptionName

Name of an exception that occurs when attempting to access outside the bounds of some data, such as beyond the end of a string.

static let undefinedKeyException: NSExceptionName

Raised when a key value coding operation fails. `userInfo` keys are described in NSUndefinedKeyException userInfo Keys

static let inconsistentArchiveException: NSExceptionName

The name of an exception raised by NSArchiver if there are problems initializing or encoding.

static let NSPPDIncludeNotFoundException: NSExceptionName

static let NSPPDIncludeStackOverflowException: NSExceptionName

static let NSPPDIncludeStackUnderflowException: NSExceptionName

static let NSPPDParseException: NSExceptionName

static let NSRTFPropertyStackOverflowException: NSExceptionName

static let NSTIFFException: NSExceptionName

static let abortModalException: NSExceptionName

static let abortPrintingException: NSExceptionName

static let accessibilityException: NSExceptionNameDeprecated

static let appKitIgnoredException: NSExceptionName

static let appKitVirtualMemoryException: NSExceptionName

static let badBitmapParametersException: NSExceptionName

static let badComparisonException: NSExceptionName

static let badRTFColorTableException: NSExceptionName

static let badRTFDirectiveException: NSExceptionName

static let badRTFFontTableException: NSExceptionName

static let badRTFStyleSheetException: NSExceptionName

static let browserIllegalDelegateException: NSExceptionName

static let colorListIOException: NSExceptionName

static let colorListNotEditableException: NSExceptionName

static let draggingException: NSExceptionName

static let fontUnavailableException: NSExceptionName

static let illegalSelectorException: NSExceptionName

static let imageCacheException: NSExceptionName

static let nibLoadingException: NSExceptionName

static let pasteboardCommunicationException: NSExceptionName

static let printOperationExistsException: NSExceptionName

The name of an exception raised when there is already a print operation in process.

static let printPackageException: NSExceptionName

static let printingCommunicationException: NSExceptionName

static let textLineTooLongException: NSExceptionName

Exception generated if a line is too long in a `NSText` object.

static let textNoSelectionException: NSExceptionName

static let textReadException: NSExceptionName

static let textWriteException: NSExceptionName

static let typedStreamVersionException: NSExceptionName

static let windowServerCommunicationException: NSExceptionName

static let wordTablesReadException: NSExceptionName

static let wordTablesWriteException: NSExceptionName

class let hierarchyInconsistencyException: NSExceptionName

Raised if the view controller hierarchy is inconsistent with the view hierarchy.

class let invalidInterfaceOrientationException: NSExceptionName

An exception that’s thrown if a view controller or the app returns an invalid set of supported interface orientations.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Related Types

typealias NSUncaughtExceptionHandler

