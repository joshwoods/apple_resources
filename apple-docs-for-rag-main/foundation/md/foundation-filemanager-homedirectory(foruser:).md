

- Foundation
- FileManager
-  homeDirectory(forUser:) 

Instance Method

# homeDirectory(forUser:)

Returns the home directory for the specified user.

macOS 10.12+

``` source
func homeDirectory(forUser userName: String) -> URL?
```

## Parameters 

`userName`  

The username of the owner of the desired home directory.

## Return Value

A URL object containing the location of the specified user’s home directory, or `nil` if no such user exists or the user’s home directory is not available.

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

func NSHomeDirectoryForUser(String?) -> String?

Returns the path to a given user’s home directory.

var temporaryDirectory: URL

The temporary directory for the current user.

func NSTemporaryDirectory() -> String

Returns the path of the temporary directory for the current user.

