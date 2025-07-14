

- Foundation
- URL Loading System
- URLCredentialStorage
-  Dictionary key for credential removal options 

API Collection

# Dictionary key for credential removal options

Key used by the options dictionary passed in remove(_:for:options:).

## Topics

### Options

let NSURLCredentialStorageRemoveSynchronizableCredentials: String

The corresponding value is an `NSNumber` object representing a Boolean value that indicates whether credentials which contain the URLCredential.Persistence.synchronizable attribute should be removed.

## See Also

### Adding and removing credentials

func remove(URLCredential, for: URLProtectionSpace)

Removes the specified credential from the credential storage for the specified protection space.

func remove(URLCredential, for: URLProtectionSpace, options: [String : Any]?)

Removes the specified credential from the credential storage for the specified protection space using the given options.

func remove(URLCredential, for: URLProtectionSpace, options: [String : Any]?, task: URLSessionTask)

Removes the specified credential from the credential storage for the specified protection space, on behalf of the given task and using the given options.

func set(URLCredential, for: URLProtectionSpace)

Adds a credential to the credential storage for the specified protection space.

func set(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Adds a credential to the credential storage for the specified protection space, on behalf of the specified task.

