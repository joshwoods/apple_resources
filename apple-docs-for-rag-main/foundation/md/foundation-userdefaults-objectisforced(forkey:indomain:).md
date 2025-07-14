

- Foundation
- UserDefaults
-  objectIsForced(forKey:inDomain:) 

Instance Method

# objectIsForced(forKey:inDomain:)

Returns a Boolean value indicating whether the key in the specified domain is managed by an administrator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func objectIsForced(
    forKey key: String,
    inDomain domain: String
) -> Bool
```

## Parameters 

`key`  

The key whose status you want to check.

`domain`  

The domain of the key.

## Return Value

true if the key is managed by an administrator in the specified domain, otherwise false.

## Discussion

This method assumes that the key is a preference associated with the current user. For managed keys, the application should disable any user interface that allows the user to modify the value of `key`.

## See Also

### Accessing Managed Environment Keys

func objectIsForced(forKey: String) -> Bool

Returns a Boolean value indicating whether the specified key is managed by an administrator.

