

- WebKit
- WKError
-  WKError.Code 

Enumeration

# WKError.Code

Possible error values that WebKit APIs can return.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
enum Code
```

## Topics

### Errors

case unknown

An error that indicates an unknown issue occurred.

case webContentProcessTerminated

An error that indicates the web process that contains the content is no longer running.

case webViewInvalidated

An error that indicates the web view was invalidated.

case javaScriptExceptionOccurred

An error that indicates a JavaScript exception occurred.

case javaScriptResultTypeIsUnsupported

An error that indicates the result of JavaScript execution could not be returned.

case contentRuleListStoreCompileFailed

An error that indicates the compilation of a rule list failed.

case contentRuleListStoreLookUpFailed

An error that indicates a content rule list data store didn’t find a rule list with the specified identifier.

case contentRuleListStoreRemoveFailed

An error that indicates a failure to remove a content rule list from the rule list data store object.

case contentRuleListStoreVersionMismatch

An error that indicates the rule list version is outdated and cannot be read.

case attributedStringContentFailedToLoad

An error that indicates the failure to navigate to web content from an attributed string.

case attributedStringContentLoadTimedOut

An error that indicates a timeout occurred while trying to load web content from an attributed string.

case javaScriptInvalidFrameTarget

An error that indicates your content referenced an invalid web frame.

case navigationAppBoundDomain

An error that indicates navigation failed due to an app-bound domain restriction.

case javaScriptAppBoundDomain

An error that indicates JavaScript execution failed due to an app-bound domain restriction.

case credentialNotFound

An error that indicates the system could not find a passkey during an export.

case duplicateCredential

An error that indicates the system found a duplicate passkey during an import.

case malformedCredential

An error that indicates the system could not parse passkey data during an import.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct WKError

Possible error values that WebKit APIs can return.

