

- WebKit
- WKError
-  navigationAppBoundDomain 

Type Property

# navigationAppBoundDomain

An error that indicates navigation failed due to an app-bound domain restriction.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static var navigationAppBoundDomain: WKError.Code { get }
```

## Discussion

This error occurs when the web view navigates away from an app-bound domain.

## See Also

### Getting the Error Codes

static var unknown: WKError.Code

An error that indicates an unknown issue occurred.

static var webContentProcessTerminated: WKError.Code

An error that indicates the web process that contains the content is no longer running.

static var webViewInvalidated: WKError.Code

An error that indicates the web view was invalidated.

static var javaScriptExceptionOccurred: WKError.Code

An error that indicates a JavaScript exception occurred.

static var javaScriptResultTypeIsUnsupported: WKError.Code

An error that indicates the result of JavaScript execution could not be returned.

static var contentRuleListStoreCompileFailed: WKError.Code

An error that indicates the compilation of a rule list failed.

static var contentRuleListStoreLookUpFailed: WKError.Code

An error that indicates a content rule list data store didn’t find a rule list with the specified identifier.

static var contentRuleListStoreRemoveFailed: WKError.Code

An error that indicates a failure to remove a content rule list from the rule list data store object.

static var contentRuleListStoreVersionMismatch: WKError.Code

An error that indicates the rule list version is outdated and cannot be read.

static var attributedStringContentFailedToLoad: WKError.Code

An error that indicates the failure to navigate to web content from an attributed string.

static var attributedStringContentLoadTimedOut: WKError.Code

An error that indicates a timeout occurred while trying to load web content from an attributed string.

static var javaScriptInvalidFrameTarget: WKError.Code

An error that indicates your content referenced an invalid web frame.

static var javaScriptAppBoundDomain: WKError.Code

An error that indicates JavaScript execution failed due to an app-bound domain restriction.

static var credentialNotFound: WKError.Code

An error that indicates the system could not find a passkey during an export.

static var duplicateCredential: WKError.Code

An error that indicates the system found a duplicate passkey during an import.

