

- Foundation
- NSURL
-  init(scheme:host:path:) Deprecated

Initializer

# init(scheme:host:path:)

Initializes a newly created NSURL with a specified scheme, host, and path.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
convenience init?(
    scheme: String,
    host: String?,
    path: String
)
```

Deprecated

Use NSURLComponents instead, which lets you create a valid URL with any valid combination of URL components and subcomponents (not just scheme, host and path), and lets you set components and subcomponents with either percent-encoded or un-percent-encoded strings.

## Parameters 

`scheme`  

The scheme for the NSURL object. For example, in the URL `http://www.example.com/index.html`, the scheme is `http`.

`host`  

The host for the NSURL object (for example, `www.example.com`). May be the empty string.

`path`  

The path for the NSURL object (for example, `/index.html`). If the path begins with a tilde, you must first expand it by calling expandingTildeInPath.

## Return Value

The newly initialized NSURL object.

## Discussion

This method automatically uses percent encoding to escape the `path` and `host` parameters.

## See Also

### Related Documentation

File System Programming Guide

URL Loading System

Interact with URLs and communicate with servers using standard Internet protocols.

