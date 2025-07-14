

- Foundation
- URLCredentialStorage
-  remove(\_:for:) 

Instance Method

# remove(\_:for:)

Removes the specified credential from the credential storage for the specified protection space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(
    _ credential: URLCredential,
    for space: URLProtectionSpace
)
```

## Parameters 

`credential`  

The credential to remove.

`space`  

The protection space from which to remove the credential.

## Discussion

If you override this method, also override remove(_:for:options:task:).

## See Also

### Adding and removing credentials

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

