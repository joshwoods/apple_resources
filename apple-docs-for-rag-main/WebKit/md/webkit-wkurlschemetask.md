

- WebKit
-  WKURLSchemeTask 

Protocol

# WKURLSchemeTask

An interface that WebKit uses to request custom resources from your app.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
protocol WKURLSchemeTask : NSObjectProtocol
```

## Overview

The WKURLSchemeTask protocol defines an interface that WebKit uses to request custom resources. You don’t adopt this interface in your own objects. Instead, WebKit creates objects that adopt this interface and delivers them to your custom scheme handlers — that is, objects that adopt the WKURLSchemeHandler protocol. You use the objects that WebKit provides to get information about the requested resources and load them. You also use those objects to report your progress back to WebKit.

When WebKit needs a custom scheme, it places an appropriate URL request in the task’s request property. Upon receiving the request, determine the size of the resource and call the didReceive(_:) method with an appropriate URL response object. Providing a response mirrors the behavior that a web server performs when it receives a request.

After you load some portion of the resource data, call the didReceive(_:) method to send it to WebKit. You may call that method multiple times to deliver data incrementally, or call it once with all of the data. After you finish delivering all of the data, call the didFinish() method. If an error occurs at any point during the load process, call didFailWithError(_:) to report it.

## Topics

### Getting the URL of the Requested Resource

var request: URLRequest

Information about the resource to load.

**Required**

### Reporting Progress Back to WebKit

func didReceive(URLResponse)

Returns a URL response to WebKit with information about the requested resource.

**Required**

func didReceive(Data)

Sends some or all of the resource data to WebKit.

**Required**

func didFinish()

Signals the successful completion of the task.

**Required**

### Reporting an Error to WebKit

func didFailWithError(any Error)

Completes the task and reports the specified error back to WebKit.

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

protocol WKURLSchemeHandler

A protocol for loading resources with URL schemes that WebKit doesn’t handle.

static let readAccessURL: NSAttributedString.DocumentReadingOptionKey

The local files WebKit can access when loading content.

