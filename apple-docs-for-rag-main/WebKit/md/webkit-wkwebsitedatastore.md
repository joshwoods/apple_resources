

- WebKit
-  WKWebsiteDataStore 

Class

# WKWebsiteDataStore

An object that manages cookies, disk and memory caches, and other types of data for a web view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
class WKWebsiteDataStore
```

## Overview

Use a WKWebsiteDataStore object to configure and manage web site data. Specifically, use this object to:

- Manage cookies that your web site uses

- Learn about the types of data that websites store

- Remove unwanted web site data

Create a data store object and assign it to the websiteDataStore property of a WKWebViewConfiguration object before you create your web view.

By default, `WKWebViewConfiguration` uses the default data store returned by the default() method, which saves website data persistently to disk.

To implement private browsing, create a nonpersistent data store using the nonPersistent() method instead.

To implement profile browsing, create a persistent data store using the init(forIdentifier:) method, passing an identifier that you use to identify the data store.

## Topics

### Creating a data store object

class func `default`() -> WKWebsiteDataStore

Returns the default data store, which stores data persistently to disk.

class func nonPersistent() -> WKWebsiteDataStore

Creates a new data store object that stores website data in memory, and doesn’t write that data to disk.

init(forIdentifier: UUID)

Returns the persistent data store with the unique identifier you provide.

### Finding data stores

class func fetchAllDataStoreIdentifiers(([UUID]) -> Void)

Fetches an array of identifiers from existing data stores that have identifiers.

### Inspecting data store properties

var identifier: UUID?

An identifier that uniquely identifies a data store.

var isPersistent: Bool

A Boolean value that indicates whether this object stores data to disk.

### Retrieving a cookie store

var httpCookieStore: WKHTTPCookieStore

The object that manages the HTTP cookies for your website.

### Retrieving specific types of data

func fetchDataRecords(ofTypes: Set&lt;String>, completionHandler: ([WKWebsiteDataRecord]) -> Void)

Fetches the specified types of records from the data store.

class func allWebsiteDataTypes() -> Set&lt;String>

Returns the set of all the available data types.

### Removing specific types of data

func removeData(ofTypes: Set&lt;String>, for: [WKWebsiteDataRecord], completionHandler: () -> Void)

Removes the specified types of website data from one or more data records.

func removeData(ofTypes: Set&lt;String>, modifiedSince: Date, completionHandler: () -> Void)

Removes website data that changed after the specified date.

### Removing a data store

class func remove(forIdentifier: UUID, completionHandler: ((any Error)?) -> Void)

Removes the data store that matches the identifier you provide.

### Instance Properties

var proxyConfigurations: [ProxyConfiguration]

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Web Data Management

class WKWebsiteDataRecord

A record of the data that a particular website stores persistently.

class WKHTTPCookieStore

An object that manages the HTTP cookies associated with a particular web view.

protocol WKURLSchemeHandler

A protocol for loading resources with URL schemes that WebKit doesn’t handle.

protocol WKURLSchemeTask

An interface that WebKit uses to request custom resources from your app.

static let readAccessURL: NSAttributedString.DocumentReadingOptionKey

The local files WebKit can access when loading content.

