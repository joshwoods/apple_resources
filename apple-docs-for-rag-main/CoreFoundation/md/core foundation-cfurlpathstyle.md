

- Core Foundation
-  CFURLPathStyle 

Enumeration

# CFURLPathStyle

Options you can use to determine how CFURL functions parse a file system path name.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFURLPathStyle
```

## Topics

### Constants

case cfurlposixPathStyle

Indicates a POSIX style path name. Components are slash delimited. A leading slash indicates an absolute path; a trailing slash is not significant.

case cfurlhfsPathStyle

Indicates a HFS style path name. Components are colon delimited. A leading colon indicates a relative path, otherwise the first path component denotes the volume.

Deprecated

case cfurlWindowsPathStyle

Indicates a Windows style path name.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Miscellaneous

enum CFURLComponentType

The types of components in a URL.

