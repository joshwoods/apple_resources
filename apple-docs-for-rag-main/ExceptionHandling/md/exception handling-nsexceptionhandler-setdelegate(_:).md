

- Exception Handling
- NSExceptionHandler
-  setDelegate(\_:) 

Instance Method

# setDelegate(\_:)

Sets the delegate of the `NSExceptionHandler` object.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setDelegate(_ anObject: Any!)
```

## Parameters 

`anObject`  

The object to receive the delegation messages described in NSExceptionHandlerDelegate

## See Also

### Getting and setting the delegate

func delegate() -> Any!

Returns the delegate of the `NSExceptionHandler` object.

