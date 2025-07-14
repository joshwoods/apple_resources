

- Foundation
-  NSHomeDirectory() 

Function

# NSHomeDirectory()

Returns the path to either the user’s or application’s home directory, depending on the platform.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSHomeDirectory() -> String
```

## Return Value

The path to the current home directory.

## Discussion

In iOS, the home directory is the application’s sandbox directory. In macOS, it’s the application’s sandbox directory, or the current user’s home directory if the application isn’t in a sandbox.

## See Also

### Accessing User Directories

var homeDirectoryForCurrentUser: URL

The home directory for the current user.

func NSUserName() -> String

Returns the logon name of the current user.

func NSFullUserName() -> String

Returns a string containing the full name of the current user.

func homeDirectory(forUser: String) -> URL?

Returns the home directory for the specified user.

func NSHomeDirectoryForUser(String?) -> String?

Returns the path to a given user’s home directory.

var temporaryDirectory: URL

The temporary directory for the current user.

func NSTemporaryDirectory() -> String

Returns the path of the temporary directory for the current user.

