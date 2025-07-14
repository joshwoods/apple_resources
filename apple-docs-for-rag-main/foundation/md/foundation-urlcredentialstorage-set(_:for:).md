

- Foundation
- URLCredentialStorage
-  set(\_:for:) 

Instance Method

# set(\_:for:)

Adds a credential to the credential storage for the specified protection space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func set(
    _ credential: URLCredential,
    for space: URLProtectionSpace
)
```

## Parameters 

`credential`  

The credential to add. If a credential with the same user name already exists in `space`, then `credential` replaces the existing object.

`space`  

The protection space to which to add the credential.

## Discussion

If the credential is not yet in the set for the protection space, it will be added to it.

If you override this method, also override set(_:for:task:).

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

func set(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Adds a credential to the credential storage for the specified protection space, on behalf of the specified task.

