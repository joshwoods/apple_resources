

- Foundation
-  NSHomeDirectoryForUser(\_:) 

Function

# NSHomeDirectoryForUser(\_:)

Returns the path to a given user’s home directory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSHomeDirectoryForUser(_ userName: String?) -> String?
```

## Parameters 

`userName`  

The name of a user.

## Return Value

The path to the home directory for the user specified by `userName`.

## Discussion

For more information on file system utilities, see Low-Level File Management Programming Topics.

## See Also

### Accessing User Directories

var homeDirectoryForCurrentUser: URL

The home directory for the current user.

func NSHomeDirectory() -> String

Returns the path to either the user’s or application’s home directory, depending on the platform.

func NSUserName() -> String

Returns the logon name of the current user.

func NSFullUserName() -> String

Returns a string containing the full name of the current user.

func homeDirectory(forUser: String) -> URL?

Returns the home directory for the specified user.

var temporaryDirectory: URL

The temporary directory for the current user.

func NSTemporaryDirectory() -> String

Returns the path of the temporary directory for the current user.

