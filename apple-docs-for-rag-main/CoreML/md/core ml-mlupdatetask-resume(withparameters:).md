

- Core ML
- MLUpdateTask
-  resume(withParameters:) 

Instance Method

# resume(withParameters:)

Resumes a model update with updated parameter values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
func resume(withParameters updateParameters: [MLParameterKey : Any])
```

## Parameters 

`updateParameters`  

Model training parameter values to replace those currently set in the update task.

## Discussion

Use this method to resume the model update task with newer parameter values. You use this method within the closures you provide in an MLUpdateProgressHandlers instance to resume the MLUpdateTask.

## See Also

### Starting and Resuming an Update

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

