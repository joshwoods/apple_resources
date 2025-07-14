

- Core Foundation
-  CFURLCopyPath(\_:) 

Function

# CFURLCopyPath(\_:)

Returns the path portion of a given URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLCopyPath(_ anURL: CFURL!) -> CFString!
```

## Parameters 

`anURL`  

The `CFURL` object to examine.

## Return Value

The path of `anURL`, or `NULL` if the URL cannot be decomposed (doesn’t conform to RFC 1808). Ownership follows the create rule. See The Create Rule.

## Discussion

This function does not resolve the URL against its base, nor does it replace percent escape sequences. This function’s return value includes any leading slash (giving the path the normal POSIX appearance), if present. If this behavior is not appropriate, use CFURLCopyStrictPath(_:_:) whose return value omits any leading slash. You may also want to use the function CFURLCopyFileSystemPath(_:_:), which returns the URL’s path as a file system path for the given path style. If the path is to be passed to file system calls, you may also want to use the function CFURLGetFileSystemRepresentation(_:_:_:_:), which returns a C string.

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

func CFURLCopyPathExtension(CFURL!) -> CFString!

Returns the path extension of a given URL.

func CFURLCopyQueryString(CFURL!, CFString!) -> CFString!

Returns the query string of a given URL.

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

