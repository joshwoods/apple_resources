

- Foundation
- FileManager
-  homeDirectoryForCurrentUser 

Instance Property

# homeDirectoryForCurrentUser

The home directory for the current user.

macOS 10.12+

``` source
var homeDirectoryForCurrentUser: URL { get }
```

## See Also

### Accessing User Directories

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

func NSTemporaryDirectory() -> String

Returns the path of the temporary directory for the current user.

