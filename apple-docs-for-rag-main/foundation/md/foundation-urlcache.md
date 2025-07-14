

- Foundation
-  URLCache 

Class

# URLCache

An object that maps URL requests to cached response objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLCache
```

## Mentioned in 

Accessing cached data

## Overview

The URLCache class implements the caching of responses to URL load requests, by mapping NSURLRequest objects to CachedURLResponse objects. It provides a composite in-memory and on-disk cache, and lets you manipulate the sizes of both the in-memory and on-disk portions. You can also control the path where cache data is persistently stored.

Note

In iOS, the on-disk cache may be purged when the system runs low on disk space, but only when your app is not running.

### Thread safety

In iOS 8 and later, and macOS 10.10 and later, URLCache is thread safe.

Although URLCache instance methods can safely be called from multiple execution contexts at the same time, be aware that methods like cachedResponse(for:) and storeCachedResponse(_:for:) have an unavoidable race condition when attempting to read or write responses for the same request.

Subclasses of URLCache must implement overridden methods in such a thread-safe manner.

### Subclassing notes

The URLCache class is meant to be used as-is, but you can subclass it when you have specific needs. For example, you might want to screen which responses are cached, or reimplement the storage mechanism for security or other reasons.

When overriding methods of this class, be aware that methods that take a `task` parameter are preferred by the system to those that do not. Therefore, you should override the task-based methods when subclassing, as follows:

- Storing responses in the cache — Override the task-based storeCachedResponse(_:for:), instead of or in addition to the request-based storeCachedResponse(_:for:).

- Getting responses from the cache — Override getCachedResponse(for:completionHandler:), instead of or in addition to cachedResponse(for:).

- Removing cached responses — Override the task-based removeCachedResponse(for:), instead of or in addition to the request-based removeCachedResponse(for:).

## Topics

### Getting and setting shared cache

class var shared: URLCache

The shared URL cache instance.

### Creating a new cache object

convenience init(memoryCapacity: Int, diskCapacity: Int, directory: URL?)

Creates a URL cache object with the specified memory and disk capacities, in the specified directory.

init(memoryCapacity: Int, diskCapacity: Int, diskPath: String?)

Creates a URL cache object with the specified values.

### Getting and storing cached objects

func cachedResponse(for: URLRequest) -> CachedURLResponse?

Returns the cached URL response in the cache for the specified URL request.

func storeCachedResponse(CachedURLResponse, for: URLRequest)

Stores a cached URL response for a specified request.

func getCachedResponse(for: URLSessionDataTask, completionHandler: (CachedURLResponse?) -> Void)

Gets the cached URL response for a data task, passing it to the provided completion handler.

func storeCachedResponse(CachedURLResponse, for: URLSessionDataTask)

Stores a cached URL response for a specified data task.

### Removing cached objects

func removeCachedResponse(for: URLRequest)

Removes the cached URL response for a specified URL request.

func removeCachedResponse(for: URLSessionDataTask)

Removes the cached URL response for a specified data task.

func removeCachedResponses(since: Date)

Clears the given cache of any cached responses since the provided date.

func removeAllCachedResponses()

Clears the receiver’s cache, removing all stored cached URL responses.

### Getting and setting on-disk cache properties

var currentDiskUsage: Int

The current size of the on-disk cache, in bytes.

var diskCapacity: Int

The capacity of the on-disk cache, in bytes.

### Getting and setting in-memory cache properties

var currentMemoryUsage: Int

The current size of the in-memory cache, in bytes.

var memoryCapacity: Int

The capacity of the in-memory cache, in bytes.

### Cache storage policies

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
- NSObjectProtocol
- Sendable

## See Also

### Cache behavior

Accessing cached data

Control how URL requests make use of previously cached data.

class CachedURLResponse

A cached response to a URL request.

