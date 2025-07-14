

- Foundation
- URL
-  homeDirectory 

Type Property

# homeDirectory

The home directory for the current user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var homeDirectory: URL { get }
```

## Discussion

This URL is the equivalent of the shell value `~/`.

Complexity: `O(1)`.

## See Also

### Accessing home and user directories

static func currentDirectory() -> URL

Returns the working directory of the current process.

static func homeDirectory(forUser: String) -> URL?

Returns the home directory for the specified user.

