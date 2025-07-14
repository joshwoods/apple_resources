

- AVFoundation
- AVAssetReader
-  canAdd(\_:) 

Instance Method

# canAdd(\_:)

Determines whether you can add the output to the asset reader.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func canAdd(_ output: AVAssetReaderOutput) -> Bool
```

## Parameters 

`output`  

The asset reader output to test.

## Return Value

true if you can add the output; otherwise, false.

## Discussion

You may only add outputs that retrieve media data from the asset that you associate with the asset reader.

## See Also

### Managing Outputs

func add(AVAssetReaderOutput)

Adds an output to the reader.

var outputs: [AVAssetReaderOutput]

The outputs from which you read media data.

