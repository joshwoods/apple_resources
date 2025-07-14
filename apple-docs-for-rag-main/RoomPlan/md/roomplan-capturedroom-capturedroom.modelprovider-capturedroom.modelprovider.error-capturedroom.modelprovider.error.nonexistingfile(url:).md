

- RoomPlan
- CapturedRoom
- CapturedRoom.ModelProvider
- CapturedRoom.ModelProvider.Error
-  CapturedRoom.ModelProvider.Error.nonExistingFile(url:) 

Case

# CapturedRoom.ModelProvider.Error.nonExistingFile(url:)

An error that indicates a model-URL query failed to return a result.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
case nonExistingFile(url: URL)
```

## Parameters 

`URL`  

The URL that references a nonexisting file.

## Discussion

This error occurs when the app hasn’t associated a URL to the attributes in a model-URL query.

## See Also

### Interpreting the error

case attributeCombinationNotSupported

An error that indicates the framework doesn’t support the attributes set in a model-URL query.

