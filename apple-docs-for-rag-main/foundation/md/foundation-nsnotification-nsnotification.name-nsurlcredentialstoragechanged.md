

- Foundation
- NSNotification
- NSNotification.Name
-  NSURLCredentialStorageChanged 

Type Property

# NSURLCredentialStorageChanged

A notification posted when the set of stored credentials changes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSURLCredentialStorageChanged: NSNotification.Name
```

## Discussion

The notification’s object is the URLCredentialStorage instance that changed. This notification does not contain a userInfo dictionary.

