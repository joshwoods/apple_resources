

- Sound Analysis
- SNAudioStreamAnalyzer
-  completeAnalysis() 

Instance Method

# completeAnalysis()

Notifies the analyzer when it receives the final audio buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func completeAnalysis()
```

## Discussion

Use this method for requests that provide final results when a stream reaches its end. The analyzer ignores any further calls to the analyze(_:atAudioFramePosition:) method.

## See Also

### Analyzing Data

func analyze(AVAudioBuffer, atAudioFramePosition: AVAudioFramePosition)

Adds a new audio buffer to the analyzer’s larger stream buffer.

