

- RoomPlan
- CapturedRoom
- CapturedRoom.ModelProvider
- CapturedRoom.ModelProvider.Error
-  CapturedRoom.ModelProvider.Error.attributeCombinationNotSupported 

Case

# CapturedRoom.ModelProvider.Error.attributeCombinationNotSupported

An error that indicates the framework doesn’t support the attributes set in a model-URL query.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
case attributeCombinationNotSupported
```

## Discussion

This error occurs for the modelFileURL(for:) function when an unsupported combination of attributes resides in the argument array.

## See Also

### Interpreting the error

case nonExistingFile(url: URL)

An error that indicates a model-URL query failed to return a result.

