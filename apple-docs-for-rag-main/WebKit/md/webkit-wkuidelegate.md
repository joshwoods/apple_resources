

- WebKit
-  WKUIDelegate 

Protocol

# WKUIDelegate

The methods for presenting native user interface elements on behalf of a webpage.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
@MainActor
protocol WKUIDelegate : NSObjectProtocol
```

## Overview

Web view user interface delegates implement this protocol to control the opening of new windows, augment the behavior of default menu items displayed when the user clicks elements, and perform other user interface-related tasks. These methods can be invoked as a result of handling JavaScript or other plug-in content. The default web view implementation assumes one window per web view, so nonconventional user interfaces might implement a user interface delegate.

## Topics

### Creating and closing the web view

func webView(WKWebView, createWebViewWith: WKWebViewConfiguration, for: WKNavigationAction, windowFeatures: WKWindowFeatures) -> WKWebView?

Creates a new web view.

func webViewDidClose(WKWebView)

Notifies your app that the DOM window closed successfully.

### Displaying UI panels

func webView(WKWebView, runJavaScriptAlertPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: () -> Void)

Displays a JavaScript alert panel.

func webView(WKWebView, runJavaScriptConfirmPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: (Bool) -> Void)

Displays a JavaScript confirm panel.

func webView(WKWebView, runJavaScriptTextInputPanelWithPrompt: String, defaultText: String?, initiatedByFrame: WKFrameInfo, completionHandler: (String?) -> Void)

Displays a JavaScript text input panel.

func webView(WKWebView, showLockdownModeFirstUseMessage: String, completionHandler: (WKDialogResult) -> Void)

Displays a custom Lockdown Mode first use message.

enum WKDialogResult

An enumeration that lists the possible ways a delegate handled displaying a custom Lockdown Mode first use dialog.

### Displaying an upload panel

func webView(WKWebView, runOpenPanelWith: WKOpenPanelParameters, initiatedByFrame: WKFrameInfo, completionHandler: ([URL]?) -> Void)

Displays a file upload panel.

class WKOpenPanelParameters

The configuration details of a file upload control in your web content.

### Displaying a contextual menu

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func webView(WKWebView, contextMenuConfigurationForElement: WKContextMenuElementInfo, completionHandler: (UIContextMenuConfiguration?) -> Void)

Tells the delegate that a contextual menu interaction began.

func webView(WKWebView, contextMenuForElement: WKContextMenuElementInfo, willCommitWithAnimator: any UIContextMenuInteractionCommitAnimating)

Provides the delegate with the animator object that the web view uses to display the contextual menu.

func webView(WKWebView, contextMenuWillPresentForElement: WKContextMenuElementInfo)

Tells the delegate that the web view is about to present the contextual menu for the specified element.

func webView(WKWebView, contextMenuDidEndForElement: WKContextMenuElementInfo)

Tells the delegate that the web view dismissed the contextual menu for the specified element.

@MainActor class UIContextMenuConfiguration

An object containing the configuration details for the contextual menu.

### Displaying an edit menu

func webView(WKWebView, willDismissEditMenuWithAnimator: any UIEditMenuInteractionAnimating)

Tells the delegate that the web view is about to dismiss an edit menu.

func webView(WKWebView, willPresentEditMenuWithAnimator: any UIEditMenuInteractionAnimating)

Tells the delegate that the web view is about to present an edit menu.

### Requesting permissions

func webView(WKWebView, requestDeviceOrientationAndMotionPermissionFor: WKSecurityOrigin, initiatedByFrame: WKFrameInfo, decisionHandler: (WKPermissionDecision) -> Void)

Determines whether a web resource, which the security origin object describes, can access the device’s orientation and motion.

func webView(WKWebView, requestMediaCapturePermissionFor: WKSecurityOrigin, initiatedByFrame: WKFrameInfo, type: WKMediaCaptureType, decisionHandler: (WKPermissionDecision) -> Void)

Determines whether a web resource, which the security origin object describes, can access to the device’s microphone audio and camera video.

enum WKPermissionDecision

An enumeration of possible permission decisions for device resource access.

enum WKMediaCaptureType

An enumeration listing the types of media devices that can capture audio, video, or both.

### Deprecated

Deprecated symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Web view

Replacing UIWebView in your app

Find a suitable alternative to handle your app’s web content.

Viewing Desktop or Mobile Web Content Using a Web View

Implement a simple iPad web browser that can view either the desktop or mobile version of a website.

class WKWebView

An object that displays interactive web content, such as for an in-app browser.

