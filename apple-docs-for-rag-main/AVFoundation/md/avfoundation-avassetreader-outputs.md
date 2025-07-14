

- AVFoundation
- AVAssetReader
-  outputs 

Instance Property

# outputs

The outputs from which you read media data.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var outputs: [AVAssetReaderOutput] { get }
```

## Discussion

The array contains the concrete instances of AVAssetReaderOutput that you associate with the reader.

## See Also

### Managing Outputs

func canAdd(AVAssetReaderOutput) -> Bool

Determines whether you can add the output to the asset reader.

func add(AVAssetReaderOutput)

Adds an output to the reader.

