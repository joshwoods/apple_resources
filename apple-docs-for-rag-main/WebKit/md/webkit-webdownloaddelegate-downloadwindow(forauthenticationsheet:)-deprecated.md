

- WebKit
- WebDownloadDelegate
-  downloadWindow(forAuthenticationSheet:) Deprecated

Instance Method

# downloadWindow(forAuthenticationSheet:)

Returns the window to be used by the authentication sheet.

macOS 10.4–10.14Deprecated

``` source
optional func downloadWindow(forAuthenticationSheet download: WebDownload!) -> NSWindow!
```

## Parameters 

`download`  

The download object that is requesting the window.

## Return Value

An NSWindow object into which the `WebDownload` object should draw its authentication sheet.

## Discussion

The default implementation prompts the user for authentication using the standard WebKit authentication panel, as either a sheet or window.

