

- Foundation
- UserDefaults
-  objectIsForced(forKey:) 

Instance Method

# objectIsForced(forKey:)

Returns a Boolean value indicating whether the specified key is managed by an administrator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func objectIsForced(forKey key: String) -> Bool
```

## Parameters 

`key`  

The key whose status you want to check.

## Return Value

true if the value of the specified key is managed by an administrator, otherwise false.

## Discussion

This method assumes that the key is a preference associated with the current user and application. For managed keys, the application should disable any user interface that allows the user to modify the value of `key`.

## See Also

### Accessing Managed Environment Keys

func objectIsForced(forKey: String, inDomain: String) -> Bool

Returns a Boolean value indicating whether the key in the specified domain is managed by an administrator.

