

- Core Foundation
- CFURLPathStyle
-  CFURLPathStyle.cfurlhfsPathStyle Deprecated

Case

# CFURLPathStyle.cfurlhfsPathStyle

Indicates a HFS style path name. Components are colon delimited. A leading colon indicates a relative path, otherwise the first path component denotes the volume.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
case cfurlhfsPathStyle
```

Deprecated

Carbon File Manager is deprecated, use kCFURLPOSIXPathStyle where possible

## See Also

### Constants

case cfurlposixPathStyle

Indicates a POSIX style path name. Components are slash delimited. A leading slash indicates an absolute path; a trailing slash is not significant.

case cfurlWindowsPathStyle

Indicates a Windows style path name.

