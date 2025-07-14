

- Foundation
- URLSessionConfiguration
-  init() Deprecated

Initializer

# init()

Creates an empty session configuration.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
init()
```

Deprecated

Use default or other class methods to create instances.

## See Also

### Creating a session configuration object

class var `default`: URLSessionConfiguration

A default session configuration object.

class var ephemeral: URLSessionConfiguration

A session configuration that uses no persistent storage for caches, cookies, or credentials.

class func background(withIdentifier: String) -> URLSessionConfiguration

Creates a session configuration object that allows HTTP and HTTPS uploads or downloads to be performed in the background.

class func new() -> Self

Creates an empty session configuration.

Deprecated

