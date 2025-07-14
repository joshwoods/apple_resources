

- WebKit
- WKWebsiteDataRecord
-  Data Store Record Types 

API Collection

# Data Store Record Types

Explore the constants that identify the types of data that websites store.

## Overview

A WKWebsiteDataRecord object includes these constants in its dataTypes property.

## Topics

### Cookie Type

let WKWebsiteDataTypeCookies: String

Cookies.

### Cache Types

let WKWebsiteDataTypeMemoryCache: String

In-memory caches.

let WKWebsiteDataTypeDiskCache: String

On-disk caches.

let WKWebsiteDataTypeOfflineWebApplicationCache: String

HTML offline web app caches.

### Storage Types

let WKWebsiteDataTypeLocalStorage: String

HTML local storage.

let WKWebsiteDataTypeSessionStorage: String

HTML session storage.

### Database Types

let WKWebsiteDataTypeWebSQLDatabases: String

WebSQL databases.

let WKWebsiteDataTypeIndexedDBDatabases: String

IndexedDB databases.

## See Also

### Getting the Data Type

var dataTypes: Set&lt;String>

The types of data associated with the record.

