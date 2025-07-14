

- Foundation
-  CachedURLResponse 

Class

# CachedURLResponse

A cached response to a URL request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CachedURLResponse
```

## Mentioned in 

Accessing cached data

## Overview

A CachedURLResponse object provides the server’s response metadata in the form of a URLResponse object, along with an NSData object containing the actual cached content data. Its storage policy determines whether the response should be cached on disk, in memory, or not at all.

Cached responses also contain a user info dictionary where you can store app-specific information about the cached item.

The URLCache class stores and retrieves instances of CachedURLResponse.

## Topics

### Creating a cached URL response

init(response: URLResponse, data: Data)

Creates a cached URL response instance.

init(response: URLResponse, data: Data, userInfo: [AnyHashable : Any]?, storagePolicy: URLCache.StoragePolicy)

Creates a cached URL response with a given server response, data, user-info dictionary, and storage policy.

### Getting cached URL response properties

var data: Data

The cached response’s data.

var response: URLResponse

The URL response object associated with the instance.

var storagePolicy: URLCache.StoragePolicy

The cached response’s storage policy.

var userInfo: [AnyHashable : Any]?

The cached response’s user info dictionary.

### Setting cache storage policies

enum StoragePolicy

These constants specify the caching strategy used by an CachedURLResponse object.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Cache behavior

Accessing cached data

Control how URL requests make use of previously cached data.

class URLCache

An object that maps URL requests to cached response objects.

