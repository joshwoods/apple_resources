

- AVFoundation
- AVExternalStorageDevice
-  nextAvailableURLs(withPathExtensions:) 

Instance Method

# nextAvailableURLs(withPathExtensions:)

Generates an array of security scoped URLs that are compliant for digital camera formats, where each element has a different path extension.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
func nextAvailableURLs(withPathExtensions extensionArray: [String]) throws -> [URL]
```

## Parameters 

`extensionArray`  

An array of path extensions the method generates URLs for.

## Return Value

An array of digital camera format (DCF) compliant URLs with security scoping, one for each path extension element in `extensionArray`.

## Discussion

The method generates a digital camera format (DCF) compliant URL with security scoping for each file extension element in `extensionArray`. It does this by configuring the folder structure and, if necessary, creates a digital camera image (DCIM) folder on the external storage device.

Important

The method generates an error if authorizationStatus isn’t AVAuthorizationStatus.authorized.

### Request access to the storage device before request

Your app can request authorization before calling the method if authorizationStatus is AVAuthorizationStatus.notDetermined by calling the requestAccess(completionHandler:) method first.

### Start and stop access to a URL around your code

To access one of the security-scoped URLs the method returns, you need to call the startAccessingSecurityScopedResource(), and stopAccessingSecurityScopedResource() methods before and after your code.

- Swift
- Objective-C

```
securityScopedURL.startAccessingSecurityScopedResource()

// Your code that accesses the URL goes in between the start and stop calls.
...

securityScopedURL.stopAccessingSecurityScopedResource()
```

```
[securityScopedURL startAccessingSecurityScopedResource];

// Your code that accesses the URL goes in between the start and stop calls.
...

[securityScopedURL stopAccessingSecurityScopedResource];

```

