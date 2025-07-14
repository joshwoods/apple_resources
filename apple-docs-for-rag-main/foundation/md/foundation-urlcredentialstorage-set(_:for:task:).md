

- Foundation
- URLCredentialStorage
-  set(\_:for:task:) 

Instance Method

# set(\_:for:task:)

Adds a credential to the credential storage for the specified protection space, on behalf of the specified task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func set(
    _ credential: URLCredential,
    for protectionSpace: URLProtectionSpace,
    task: URLSessionTask
)
```

## Parameters 

`credential`  

The credential to add. If a credential with the same user name already exists in `space`, then `credential` replaces the existing object.

`protectionSpace`  

The protection space to which to add the credential.

`task`  

The task accessing the specified protection space. Subclasses of URLCredentialStorage may use the request URL or other properties of this task to affect how the default credential is stored.

## See Also

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

