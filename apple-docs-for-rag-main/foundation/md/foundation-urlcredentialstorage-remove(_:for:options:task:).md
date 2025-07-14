

- Foundation
- URLCredentialStorage
-  remove(\_:for:options:task:) 

Instance Method

# remove(\_:for:options:task:)

Removes the specified credential from the credential storage for the specified protection space, on behalf of the given task and using the given options.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(
    _ credential: URLCredential,
    for protectionSpace: URLProtectionSpace,
    options: [String : Any]? = nil,
    task: URLSessionTask
)
```

## Parameters 

`credential`  

The credential to remove.

`protectionSpace`  

The protection space from which to remove the credential.

`options`  

A dictionary containing options to consider when removing the credential.

For possible keys, see Dictionary key for credential removal options. You should use this when trying to delete a credential that has the URLCredential.Persistence.synchronizable policy.

Note

When credential objects that have a `synchronizable` policy are removed, the credential will be removed on all devices that contain this credential.

`task`  

The task using the protection space that you wish to remove the credential for.

## Discussion

The credential is removed from both persistent and temporary storage.

## See Also

### Adding and removing credentials

func remove(URLCredential, for: URLProtectionSpace)

Removes the specified credential from the credential storage for the specified protection space.

func remove(URLCredential, for: URLProtectionSpace, options: [String : Any]?)

Removes the specified credential from the credential storage for the specified protection space using the given options.

Dictionary key for credential removal options

Key used by the options dictionary passed in remove(_:for:options:).

func set(URLCredential, for: URLProtectionSpace)

Adds a credential to the credential storage for the specified protection space.

func set(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Adds a credential to the credential storage for the specified protection space, on behalf of the specified task.

