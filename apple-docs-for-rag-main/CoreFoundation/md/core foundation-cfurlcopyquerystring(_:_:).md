

- Core Foundation
-  CFURLCopyQueryString(\_:\_:) 

Function

# CFURLCopyQueryString(\_:\_:)

Returns the query string of a given URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLCopyQueryString(
    _ anURL: CFURL!,
    _ charactersToLeaveEscaped: CFString!
) -> CFString!
```

## Parameters 

`anURL`  

The `CFURL` object to examine.

`charactersToLeaveEscaped`  

Characters whose percent escape sequences, such as `%20` for a space character, you want to leave intact. Pass `NULL` to specify that no percent escapes be replaced, or the empty string (`CFSTR("")`) to specify that all be replaced.

## Return Value

The query string, or `NULL` if no parameter string exists. Ownership follows the create rule. See The Create Rule.

## Discussion

This function removes all percent escape sequences except those for characters specified in `charactersToLeaveEscaped`.

## See Also

### Accessing the Parts of a URL

func CFURLCanBeDecomposed(CFURL!) -> Bool

Determines if the given URL conforms to RFC 1808 and therefore can be decomposed.

func CFURLCopyFileSystemPath(CFURL!, CFURLPathStyle) -> CFString!

Returns the path portion of a given URL.

func CFURLCopyFragment(CFURL!, CFString!) -> CFString!

Returns the fragment from a given URL.

func CFURLCopyHostName(CFURL!) -> CFString!

Returns the host name of a given URL.

func CFURLCopyLastPathComponent(CFURL!) -> CFString!

Returns the last path component of a given URL.

func CFURLCopyNetLocation(CFURL!) -> CFString!

Returns the net location portion of a given URL.

func CFURLCopyParameterString(CFURL!, CFString!) -> CFString!

Returns the parameter string from a given URL.

Deprecated

func CFURLCopyPassword(CFURL!) -> CFString!

Returns the password of a given URL.

func CFURLCopyPath(CFURL!) -> CFString!

Returns the path portion of a given URL.

func CFURLCopyPathExtension(CFURL!) -> CFString!

Returns the path extension of a given URL.

func CFURLCopyResourceSpecifier(CFURL!) -> CFString!

Returns any additional resource specifiers after the path.

func CFURLCopyScheme(CFURL!) -> CFString!

Returns the scheme portion of a given URL.

func CFURLCopyStrictPath(CFURL!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> CFString!

Returns the path portion of a given URL.

func CFURLCopyUserName(CFURL!) -> CFString!

Returns the user name from a given URL.

func CFURLGetPortNumber(CFURL!) -> Int32

Returns the port number from a given URL.

