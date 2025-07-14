

- WebKit
-  WKURLSchemeHandler 

Protocol

# WKURLSchemeHandler

A protocol for loading resources with URL schemes that WebKit doesn’t handle.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
protocol WKURLSchemeHandler : NSObjectProtocol
```

## Overview

Adopt the WKURLSchemeHandler protocol in objects that handle custom URL schemes for your web content. Custom schemes let you integrate custom resource types into your web content, and you may define custom schemes for resources that your app requires. For example, you might use a custom scheme to integrate content that is available only on the user’s device, such as the user’s photos. Adopt this protocol in one of your app’s objects and register it using the setURLSchemeHandler(_:forURLScheme:) method of WKWebViewConfiguration.

When a web view encounters a resource that uses a custom scheme, it creates a WKURLSchemeTask object and passes it to the methods of your scheme handler object. Use the webView(_:start:) method to begin loading the resource. While your handler loads the object, the web view may call your handler’s webView(_:stop:) method to notify you that the resource is no longer needed.

## Topics

### Loading a Custom Resource

func webView(WKWebView, start: any WKURLSchemeTask)

Asks your handler to begin loading the data for the specified resource.

**Required**

### Responding to a Canceled Resource Request

func webView(WKWebView, stop: any WKURLSchemeTask)

Asks your handler to stop loading the data for the specified resource.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Web Data Management

class WKWebsiteDataStore

An object that manages cookies, disk and memory caches, and other types of data for a web view.

class WKWebsiteDataRecord

A record of the data that a particular website stores persistently.

class WKHTTPCookieStore

An object that manages the HTTP cookies associated with a particular web view.

protocol WKURLSchemeTask

An interface that WebKit uses to request custom resources from your app.

static let readAccessURL: NSAttributedString.DocumentReadingOptionKey

The local files WebKit can access when loading content.

