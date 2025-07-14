

- AVFoundation
- AVAssetReader
-  add(\_:) 

Instance Method

# add(\_:)

Adds an output to the reader.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func add(_ output: AVAssetReaderOutput)
```

## Parameters 

`output`  

The asset reader output to add.

## Discussion

Add outputs to read from one or more tracks of an asset. You can only add outputs that retrieve media data from the asset that you associate with the asset reader.

You can’t add an output after you start reading.

## See Also

### Managing Outputs

func canAdd(AVAssetReaderOutput) -> Bool

Determines whether you can add the output to the asset reader.

var outputs: [AVAssetReaderOutput]

The outputs from which you read media data.

