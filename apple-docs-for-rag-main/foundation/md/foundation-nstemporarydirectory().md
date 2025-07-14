

- Foundation
-  NSTemporaryDirectory() 

Function

# NSTemporaryDirectory()

Returns the path of the temporary directory for the current user.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSTemporaryDirectory() -> String
```

## Return Value

A string containing the path of the temporary directory for the current user.

## Discussion

See the FileManager method url(for:in:appropriateFor:create:) for the preferred means of finding the correct temporary directory.

For more information about temporary files, see File System Programming Guide.

## See Also

### Related Documentation

func NSSearchPathForDirectoriesInDomains(FileManager.SearchPathDirectory, FileManager.SearchPathDomainMask, Bool) -> [String]

Creates a list of directory search paths.

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

func NSHomeDirectoryForUser(String?) -> String?

Returns the path to a given user’s home directory.

var temporaryDirectory: URL

The temporary directory for the current user.

