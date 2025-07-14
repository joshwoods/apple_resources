

- Foundation
- URLCredentialStorage
-  remove(\_:for:options:) 

Instance Method

# remove(\_:for:options:)

Removes the specified credential from the credential storage for the specified protection space using the given options.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(
    _ credential: URLCredential,
    for space: URLProtectionSpace,
    options: [String : Any]? = nil
)
```

## Parameters 

`credential`  

The credential to remove.

`space`  

The protection space from which to remove the credential.

`options`  

A dictionary containing options to consider when removing the credential.

For possible keys, see Dictionary key for credential removal options. You should use this when trying to delete a credential that has the URLCredential.Persistence.synchronizable policy.

Note

When credential objects that have a URLCredential.Persistence.synchronizable policy are removed, the credential will be removed on all devices that contain this credential.

## Discussion

The credential is removed from both persistent and temporary storage.

If you override this method, also override remove(_:for:options:task:).

## See Also

### Adding and removing credentials

func remove(URLCredential, for: URLProtectionSpace)

Removes the specified credential from the credential storage for the specified protection space.

func remove(URLCredential, for: URLProtectionSpace, options: [String : Any]?, task: URLSessionTask)

Removes the specified credential from the credential storage for the specified protection space, on behalf of the given task and using the given options.

Dictionary key for credential removal options

Key used by the options dictionary passed in remove(_:for:options:).

func set(URLCredential, for: URLProtectionSpace)

Adds a credential to the credential storage for the specified protection space.

func set(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Adds a credential to the credential storage for the specified protection space, on behalf of the specified task.

