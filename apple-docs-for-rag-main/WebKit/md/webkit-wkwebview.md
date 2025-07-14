

- WebKit
-  WKWebView 

Class

# WKWebView

An object that displays interactive web content, such as for an in-app browser.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKWebView
```

## Mentioned in 

Replacing UIWebView in your app

## Overview

A WKWebView object is a platform-native view that you use to incorporate web content seamlessly into your app’s UI. A web view supports a full web-browsing experience, and presents HTML, CSS, and JavaScript content alongside your app’s native views. Use it when web technologies satisfy your app’s layout and styling requirements more readily than native views. For example, you might use it when your app’s content changes frequently.

A web view offers control over the navigation and user experience through delegate objects. Use the navigation delegate to react when the user clicks links in your web content, or interacts with the content in a way that affects navigation. For example, you might prevent the user from navigating to new content unless specific conditions are met. Use the UI delegate to present native UI elements, such as alerts or contextual menus, in response to interactions with your web content.

Note

WKWebView replaces the UIWebView class in iOS 8 and later, and it replaces the WebView class in macOS 10.10 and later.

Embed a WKWebView object programmatically into your view hierarchy, or add it using Interface Builder. Interface Builder supports many customizations, such as configuring data detectors, media playback, and interaction behaviors. For more extensive customizations, create your web view programmatically using a WKWebViewConfiguration object. For example, use a web view configuration object to specify handlers for custom URL schemes, manage cookies, and customize preferences for your web content.

Before your web view appears onscreen, load content from a web server using a URLRequest structure or load content directly from a local file or HTML string. The web view automatically loads embedded resources such as images or videos as part of the initial load request. It then renders your content and displays the results inside the view’s bounds rectangle. The following code example shows a view controller that replaces its default view with a custom WKWebView object.

```
import UIKit
import WebKit

class ViewController: UIViewController, WKUIDelegate {

    var webView: WKWebView!

    override func loadView() {
        let webConfiguration = WKWebViewConfiguration()
        webView = WKWebView(frame: .zero, configuration: webConfiguration)
        webView.uiDelegate = self
        view = webView
    }

    override func viewDidLoad() {
        super.viewDidLoad()

        let myURL = URL(string:"https://www.apple.com")
        let myRequest = URLRequest(url: myURL!)
        webView.load(myRequest)
    }
}
```

A web view automatically converts telephone numbers that appear in web content to Phone links. When the user taps a Phone link, the Phone app launches and dials the number. Use the WKWebViewConfiguration object to change the default data detector behavior.

You can also use setMagnification(_:centeredAt:) to programmatically set the scale of web content the first time it appears in a web view. Thereafter, the user can change the scale using gestures.

### Manage the navigation through your web content

WKWebView provides a complete browsing experience, including the ability to navigate between different webpages using links, forward and back buttons, and more. When the user clicks a link in your content, the web view acts like a browser and displays the content at that link. To disallow navigation, or to customize your web view’s navigation behavior, provide your web view with a navigation delegate — an object that conforms to the WKNavigationDelegate protocol. Use your navigation delegate to modify the web view’s navigation behavior, or to track the loading progress of new content.

You can also use the methods of WKWebView to navigate programmatically through your content, or to trigger navigation from other parts of your app’s interface. For example, if your UI includes forward and back buttons, connect those buttons to the goBack(_:) and goForward(_:) methods of your web view to trigger the corresponding web navigation. Use the canGoBack and canGoForward properties to determine when to enable or disable your buttons.

### Provide sharing options

People may want to share the contents of your web view with an app or other people. Use a UIActivityViewController to present a share sheet offering all the ways people can share the web content.

If your app has the com.apple.developer.web-browser entitlement, the iOS share sheet can offer Add to Home Screen for an `http` or `https` webpage, creating a convenient link to a web app or bookmark. To allow someone to add the current webpage to the Home Screen, include the WKWebView instance in the `activityItems` array when you call init(activityItems:applicationActivities:) to create the UIActivityViewController. For more information about building a browser app, see Preparing your app to be the default web browser.

## Topics

### Creating a web view

init(frame: CGRect, configuration: WKWebViewConfiguration)

Creates a web view and initializes it with the specified frame and configuration data.

init?(coder: NSCoder)

Returns an object initialized from data in the specified coder object.

var configuration: WKWebViewConfiguration

The object that contains the configuration details for the web view.

### Determining whether WebKit can load content

class func handlesURLScheme(String) -> Bool

Returns a Boolean value that indicates whether WebKit natively supports resources with the specified URL scheme.

### Displaying native user interface elements

var uiDelegate: (any WKUIDelegate)?

The object you use to integrate custom user interface elements, such as contextual menus or panels, into web view interactions.

protocol WKUIDelegate

The methods for presenting native user interface elements on behalf of a webpage.

### Managing navigation between webpages

var navigationDelegate: (any WKNavigationDelegate)?

The object you use to manage navigation behavior for the web view.

protocol WKNavigationDelegate

Methods for accepting or rejecting navigation changes, and for tracking the progress of navigation requests.

### Loading web content

func load(URLRequest) -> WKNavigation?

Loads the web content that the specified URL request object references and navigates to that content.

func load(Data, mimeType: String, characterEncodingName: String, baseURL: URL) -> WKNavigation?

Loads the content of the specified data object and navigates to it.

func loadHTMLString(String, baseURL: URL?) -> WKNavigation?

Loads the contents of the specified HTML string and navigates to it.

func loadFileRequest(URLRequest, allowingReadAccessTo: URL) -> WKNavigation

Loads the web content from the file the URL request object specifies and navigates to that content.

func loadFileURL(URL, allowingReadAccessTo: URL) -> WKNavigation?

Loads the web content from the specified file and navigates to it.

func loadSimulatedRequest(URLRequest, response: URLResponse, responseData: Data) -> WKNavigation

Loads the web content from the data you provide as if the data were the response to the request.

func loadSimulatedRequest(URLRequest, responseHTML: String) -> WKNavigation

Loads the web content from the HTML you provide as if the HTML were the response to the request.

var isLoading: Bool

A Boolean value that indicates whether the view is currently loading content.

var estimatedProgress: Double

An estimate of what fraction of the current navigation has been loaded.

### Managing the loading process

func reload() -> WKNavigation?

Reloads the current webpage.

func reload(Any?)

Reloads the current webpage.

func reloadFromOrigin() -> WKNavigation?

Reloads the current webpage, and performs end-to-end revalidation of the content using cache-validating conditionals, if possible.

func reloadFromOrigin(Any?)

Reloads the current webpage, and performs end-to-end revalidation of the content using cache-validating conditionals, if possible.

func stopLoading()

Stops loading all resources on the current page.

func stopLoading(Any?)

Stops loading all resources on the current page.

### Managing downloads

func startDownload(using: URLRequest, completionHandler: (WKDownload) -> Void)

Starts to download the resource at the URL in the request.

func resumeDownload(fromResumeData: Data, completionHandler: (WKDownload) -> Void)

Resumes a failed or canceled download.

### Making web content inspectable

var isInspectable: Bool

A Boolean value that indicates whether you can inspect the view with Safari Web Inspector.

### Inspecting the view information

var scrollView: UIScrollView

The scroll view associated with the web view.

var title: String?

The page title.

var url: URL?

The URL for the current webpage.

var mediaType: String?

The media type for the contents of the web view.

var customUserAgent: String?

The custom user agent string.

var serverTrust: SecTrust?

The trust management object you use to evaluate trust for the current webpage.

var hasOnlySecureContent: Bool

A Boolean value that indicates whether the web view loaded all resources on the page through securely encrypted connections.

var themeColor: UIColor?

The theme color that the system gets from the first valid meta tag in the webpage.

var underPageBackgroundColor: UIColor!

The color the web view displays behind the active page, visible when the user scrolls beyond the bounds of the page.

### Scaling content

var pageZoom: CGFloat

The scale factor by which the web view scales content relative to its bounds.

var allowsMagnification: Bool

A Boolean value that indicates whether magnify gestures change the web view’s magnification.

var magnification: CGFloat

The factor by which the page content is currently scaled.

func setMagnification(CGFloat, centeredAt: CGPoint)

Scales the page content and centers the result on the specified point.

### Interacting with media

func pauseAllMediaPlayback(completionHandler: (() -> Void)?)

Pauses playback of all media in the web view.

func requestMediaPlaybackState(completionHandler: (WKMediaPlaybackState) -> Void)

Requests the playback status of media in the web view.

func setAllMediaPlaybackSuspended(Bool, completionHandler: (() -> Void)?)

Changes whether the webpage is suspending playback of all media in the page.

func closeAllMediaPresentations(completionHandler: (() -> Void)?)

Closes all media the web view is presenting, including picture-in-picture video and fullscreen video.

enum WKMediaPlaybackState

An enumeration that describes whether an audio or video presentation is playing, paused, or suspended.

### Managing the microphone and camera

var cameraCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the camera to capture images or video.

var microphoneCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the microphone to capture audio.

func setCameraCaptureState(WKMediaCaptureState, completionHandler: (() -> Void)?)

Changes whether the webpage is using the camera to capture images or video.

func setMicrophoneCaptureState(WKMediaCaptureState, completionHandler: (() -> Void)?)

Changes whether the webpage is using the microphone to capture audio.

enum WKMediaCaptureState

An enumeration that describes whether a media device, like a camera or microphone, is currently capturing audio or video.

### Searching the current page’s content

func find(String, configuration: WKFindConfiguration, completionHandler: (WKFindResult) -> Void)

Searches for the specified string in the web view’s content.

func find(String, configuration: WKFindConfiguration) async throws -> WKFindResult

Searches for the specified string in the web view’s content.

class WKFindConfiguration

The configuration parameters to use when searching the contents of the web view.

class WKFindResult

An object that contains the results of searching the web view’s contents.

### Navigating between webpages

var allowsBackForwardNavigationGestures: Bool

A Boolean value that indicates whether horizontal swipe gestures trigger backward and forward page navigation.

var backForwardList: WKBackForwardList

The web view’s back-forward list.

func goBack(Any?)

Navigates to the back item in the back-forward list.

func goBack() -> WKNavigation?

Navigates to the back item in the back-forward list.

func goForward(Any?)

Navigates to the forward item in the back-forward list.

func goForward() -> WKNavigation?

Navigates to the forward item in the back-forward list.

func go(to: WKBackForwardListItem) -> WKNavigation?

Navigates to an item from the back-forward list and sets it as the current item.

var canGoBack: Bool

A Boolean value that indicates whether there is a valid back item in the back-forward list.

var canGoForward: Bool

A Boolean value that indicates whether there is a valid forward item in the back-forward list.

var allowsLinkPreview: Bool

A Boolean value that determines whether pressing a link displays a preview of the destination for the link.

var interactionState: Any?

An object you use to capture the current state of interaction in a web view so that you can restore that state later to another web view.

### Executing JavaScript

func evaluateJavaScript(String, completionHandler: ((Any?, (any Error)?) -> Void)?)

Evaluates the specified JavaScript string.

func evaluateJavaScript(String, in: WKFrameInfo?, in: WKContentWorld, completionHandler: ((Result&lt;Any, any Error>) -> Void)?)

Evaluates a JavaScript string in the context of the specified frame and content world.

func evaluateJavaScript(String, in: WKFrameInfo?, contentWorld: WKContentWorld) async throws -> Any?

Evaluates a JavaScript string in the context of the specified frame and content world.

func callAsyncJavaScript(String, arguments: [String : Any], in: WKFrameInfo?, in: WKContentWorld, completionHandler: ((Result&lt;Any, any Error>) -> Void)?)

Executes the specified string as an asynchronous JavaScript function.

func callAsyncJavaScript(String, arguments: [String : Any], in: WKFrameInfo?, contentWorld: WKContentWorld) async throws -> Any?

Executes the specified string as an asynchronous JavaScript function.

### Capturing the web view’s content

func takeSnapshot(with: WKSnapshotConfiguration?, completionHandler: (UIImage?, (any Error)?) -> Void)

Generates a platform-native image from the web view’s contents asynchronously.

func createPDF(configuration: WKPDFConfiguration, completionHandler: (Result&lt;Data, any Error>) -> Void)

Generates PDF data from the web view’s contents asynchronously.

func pdf(configuration: WKPDFConfiguration) async throws -> Data

Generates PDF data from the web view’s contents asynchronously.

func createWebArchiveData(completionHandler: (Result&lt;Data, any Error>) -> Void)

Creates a web archive of the web view’s current contents asynchronously.

func printOperation(with: NSPrintInfo) -> NSPrintOperation

Returns the print operation object to use when printing the contents of the web view.

class WKSnapshotConfiguration

The configuration data to use when generating an image from a web view’s contents.

class WKPDFConfiguration

The configuration data to use when generating a PDF representation of a web view’s contents.

### Supporting Find and Replace

var isFindInteractionEnabled: Bool

var findInteraction: UIFindInteraction?

### Handling full-screen transitions

var fullscreenState: WKWebView.FullscreenState

enum FullscreenState

### Configuring viewport insets

func setMinimumViewportInset(UIEdgeInsets, maximumViewportInset: UIEdgeInsets)

var minimumViewportInset: UIEdgeInsets

var maximumViewportInset: UIEdgeInsets

### Deprecated

Deprecated symbols

Review unsupported symbols and their replacements.

### Instance Properties

var isWritingToolsActive: Bool

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTextFinderClient
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Web view

Replacing UIWebView in your app

Find a suitable alternative to handle your app’s web content.

Viewing Desktop or Mobile Web Content Using a Web View

Implement a simple iPad web browser that can view either the desktop or mobile version of a website.

protocol WKUIDelegate

The methods for presenting native user interface elements on behalf of a webpage.

