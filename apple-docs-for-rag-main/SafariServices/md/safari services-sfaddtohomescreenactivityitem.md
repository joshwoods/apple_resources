

- Safari Services
-  SFAddToHomeScreenActivityItem 

Protocol

# SFAddToHomeScreenActivityItem

A protocol that describes a bookmark someone can add to their Home Screen.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+

``` source
protocol SFAddToHomeScreenActivityItem : NSObjectProtocol
```

## Overview

To add a bookmark to someone’s Home Screen from your browser app, create an object that conforms to SFAddToHomeScreenActivityItem and present a UIActivityViewController that includes the activity item.

If your browser app uses WebKit, SFAddToHomeScreenActivityItem always represents a bookmark. To let someone add a web app to their Home Screen, add a WKWebView to the UIActivityViewController activity items instead of a SFAddToHomeScreenActivityItem. WebKit inspects the website’s metadata to decide whether the item represents a bookmark or a web app.

If your browser app includes an alternative browser engine, pass detailed information about the bookmark to getHomeScreenWebAppInfo(completionHandler:). If the bookmark represents a web app, include the web app manifest, and cookies that the system uses when someone opens the web app from their Home Screen.

Important

SFAddToHomeScreenActivityItem is only available to web browsers. For more information on creating a web browser, see Preparing your app to be the default web browser.

## Topics

### Describing a bookmark or web app

var iconItemProvider: NSItemProvider?

An object that conveys the bookmark’s icon to the system.

var title: String

The bookmark’s title.

**Required**

var url: URL

The bookmark’s URL.

**Required**

### Providing information about a web app to the system

func getHomeScreenWebAppInfo(completionHandler: (SFAddToHomeScreenInfo?) -> Void)

Provides information about a web app to the system.

class SFAddToHomeScreenInfo

A class that provides information about a web app that someone adds to their Home Screen.

func getWebAppManifest(completionHandler: (BEWebAppManifest?) -> Void)

Provides the web app’s manifest to the system, if the bookmark represents a web app.

## Relationships

### Inherits From

- NSObjectProtocol

