

- TVMLKit JS
- NSError
-  userInfo 

Instance Property

# userInfo

The user info dictionary.

tvOS 11.0+

``` source
readonly attribute Object userInfo;
```

## Discussion

If the user info dictionary has not been set, this property is `nil`.

## See Also

### Getting Error Properties

code

The error code.

domain

A string containing the error domain.

underlyingError

The error that was encountered in an underlying implementation and caused the error that the receiver represents to occur.

