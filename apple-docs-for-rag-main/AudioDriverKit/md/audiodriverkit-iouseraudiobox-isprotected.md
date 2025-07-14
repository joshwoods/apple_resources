

- AudioDriverKit
- IOUserAudioBox
-  IsProtected 

Instance Method

# IsProtected

Returns a Boolean value that indicates if the box requires authentication before use.

DriverKit 21.0+

``` source
bool IsProtected();
```

## Return Value

`true` if the box is protected; `false` otherwise.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Managing Protection State

SetIsProtected

Sets a Boolean value that indicates if the box requires authentication before use.

