

- Foundation
-  URLCredentialStorage 

Class

# URLCredentialStorage

The manager of a shared credentials cache.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLCredentialStorage
```

## Overview

The shared cache stores and retrieves instances of URLCredential. You can store password-based credentials permanently, based on the URLCredential.Persistence they were created with. Certificate-based credentials are never stored permanently.

### Subclassing notes

The URLCredentialStorage class is meant to be used as-is, but you can subclass it if you have specific needs, such as screening which credentials are stored.

When overriding methods of this class, be aware that methods that take a `task` parameter are preferred to equivalent methods that do not. Therefore, you should override the task-based methods when subclassing, as follows:

- Setting credentials — Override set(_:for:task:) instead of or in addition to set(_:for:).

- Getting credentials — Override getCredentials(for:task:completionHandler:) instead of or in addition to credentials(for:).

- Removing credentials — Override remove(_:for:options:task:) instead of or in addition to remove(_:for:options:) and remove(_:for:).

- Setting default credentials — Override setDefaultCredential(_:for:task:) instead of or in addition to setDefaultCredential(_:for:).

- Getting default credentials — Override getDefaultCredential(for:task:completionHandler:) instead of or in addition to defaultCredential(for:).

## Topics

### Getting the credential storage

class var shared: URLCredentialStorage

The shared URL credential storage instance.

### Getting and setting default credentials

func defaultCredential(for: URLProtectionSpace) -> URLCredential?

Returns the default credential for the specified protection space.

func getDefaultCredential(for: URLProtectionSpace, task: URLSessionTask, completionHandler: (URLCredential?) -> Void)

Gets the default credential for the specified protection space, which is being accessed by the given task, and passes it to the provided completion handler.

func setDefaultCredential(URLCredential, for: URLProtectionSpace)

Sets the default credential for a specified protection space.

func setDefaultCredential(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Sets the default credential for a given protection space, which is being accessed by the given task.

### Adding and removing credentials

func remove(URLCredential, for: URLProtectionSpace)

Removes the specified credential from the credential storage for the specified protection space.

func remove(URLCredential, for: URLProtectionSpace, options: [String : Any]?)

Removes the specified credential from the credential storage for the specified protection space using the given options.

func remove(URLCredential, for: URLProtectionSpace, options: [String : Any]?, task: URLSessionTask)

Removes the specified credential from the credential storage for the specified protection space, on behalf of the given task and using the given options.

Dictionary key for credential removal options

Key used by the options dictionary passed in remove(_:for:options:).

func set(URLCredential, for: URLProtectionSpace)

Adds a credential to the credential storage for the specified protection space.

func set(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Adds a credential to the credential storage for the specified protection space, on behalf of the specified task.

### Retrieving credentials

var allCredentials: [URLProtectionSpace : [String : URLCredential]]

The credentials for all available protection spaces.

func credentials(for: URLProtectionSpace) -> [String : URLCredential]?

Returns a dictionary containing the credentials for the specified protection space.

func getCredentials(for: URLProtectionSpace, task: URLSessionTask, completionHandler: ([String : URLCredential]?) -> Void)

Gets a dictionary containing the credentials for the specified protection space, on behalf of the given task, and passes the dictionary to the provided completion handler.

### Tracking credential storage changes

static let NSURLCredentialStorageChanged: NSNotification.Name

A notification posted when the set of stored credentials changes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Authentication and credentials

Handling an authentication challenge

Respond appropriately when a server demands authentication for a URL request.

class URLAuthenticationChallenge

A challenge from a server requiring authentication from the client.

class URLCredential

`A`n authentication credential consisting of information specific to the type of credential and the type of persistent storage to use, if any.

class URLProtectionSpace

A server or an area on a server, commonly referred to as a realm, that requires authentication.

