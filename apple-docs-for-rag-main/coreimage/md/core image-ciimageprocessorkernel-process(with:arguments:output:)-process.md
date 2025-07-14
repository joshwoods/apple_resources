

- Core Image
- CIImageProcessorKernel
-  process(with:arguments:output:) 

Type Method

# process(with:arguments:output:)

Method to override for customizing the kernel's image processing.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class func process(
    with inputs: [any CIImageProcessorInput]?,
    arguments: [String : Any]?,
    output: any CIImageProcessorOutput
) throws
```

## Parameters 

`inputs`  

Inputs to this processor stage.

`arguments`  

Dictionary of arguments mapping keys such as `"thresholdValue"` to their values.

`output`  

The output image following processing.

`error`  

Pointer to the NSError object into which processing errors will be written.

## Return Value

Returns `true` if processing succeeded, and `false` if processing failed.

## Discussion

Override this method to perform custom image processing.

