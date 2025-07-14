

- Foundation
- URL
-  homeDirectory(forUser:) 

Type Method

# homeDirectory(forUser:)

Returns the home directory for the specified user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func homeDirectory(forUser user: String) -> URL?
```

## Parameters 

`user`  

The system user name for a given user.

## Return Value

The home directory for the specified user.

## See Also

### Accessing home and user directories

static func currentDirectory() -> URL

Returns the working directory of the current process.

static var homeDirectory: URL

The home directory for the current user.

