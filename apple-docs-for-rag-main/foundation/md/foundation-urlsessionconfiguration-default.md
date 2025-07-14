

- Foundation
- URLSessionConfiguration
-  default 

Type Property

# default

A default session configuration object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var `default`: URLSessionConfiguration { get }
```

## Discussion

The default session configuration uses a persistent disk-based cache (except when the result is downloaded to a file) and stores credentials in the user’s keychain. It also stores cookies (by default) in the same shared cookie store as the NSURLConnection and NSURLDownload classes.

Note

If you’re porting code based on the NSURLConnection class, use this method to obtain an initial configuration object and then customize that object as needed.

Modifying the returned session configuration object does *not* affect any configuration objects returned by future calls to this method, and does not change the default behavior for existing sessions. It is therefore always safe to use the returned object as a starting point for additional customization.

## See Also

### Related Documentation

Fetching website data into memory

Receive data directly into memory by creating a data task from a URL session.

### Creating a session configuration object

class var ephemeral: URLSessionConfiguration

A session configuration that uses no persistent storage for caches, cookies, or credentials.

class func background(withIdentifier: String) -> URLSessionConfiguration

Creates a session configuration object that allows HTTP and HTTPS uploads or downloads to be performed in the background.

init()

Creates an empty session configuration.

Deprecated

class func new() -> Self

Creates an empty session configuration.

Deprecated

