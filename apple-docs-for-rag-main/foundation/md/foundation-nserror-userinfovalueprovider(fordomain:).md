

- Foundation
- NSError
-  userInfoValueProvider(forDomain:) 

Type Method

# userInfoValueProvider(forDomain:)

Returns any user info provider specified for a given error domain.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func userInfoValueProvider(forDomain errorDomain: String) -> ((any Error, String) -> Any?)?
```

## Parameters 

`errorDomain`  

The error domain of the user info provider.

## Return Value

The user info provider of the error domain, or `nil` if none is specified.

## See Also

### Providing Error User Info

class func setUserInfoValueProvider(forDomain: String, provider: ((any Error, String) -> Any?)?)

Specifies a block to call when the corresponding property is not present in the user info dictionary.

struct ErrorUserInfoKey

typealias UserInfoKey

These keys may exist in the user info dictionary.

