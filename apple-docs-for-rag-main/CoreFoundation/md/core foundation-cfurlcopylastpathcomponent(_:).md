

- Core Foundation
-  CFURLCopyLastPathComponent(\_:) 

Function

# CFURLCopyLastPathComponent(\_:)

Returns the last path component of a given URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLCopyLastPathComponent(_ url: CFURL!) -> CFString!
```

## Parameters 

`url`  

The `CFURL` object to examine.

## Return Value

The last path component of `url`. Ownership follows the create rule. See The Create Rule.

## Discussion

Note that if there is no last path component, this function returns an empty string. In the code sample shown, `lastPathComponent` is an empty string.

```
CFStringRef urlString = CFSTR("http://www.apple.com");
CFURLRef url = CFURLCreateWithString(NULL, urlString, NULL);
CFStringRef lastPathComponent = CFURLCopyLastPathComponent (url);
```

If `urlString` were created with `CFSTR("http://www.apple.com/")`, then `lastPathComponent` would be a `CFString` object containing the character “`/`”.

See also CFURLCopyPathExtension(_:).

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

