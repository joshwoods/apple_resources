

- AVFAudio
- AVAudio3DMixing
-  renderingAlgorithm 

Instance Property

# renderingAlgorithm

The type of rendering algorithm the mixer uses.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+

``` source
var renderingAlgorithm: AVAudio3DMixingRenderingAlgorithm { get set }
```

**Required**

## Discussion

Depending on the current output format of the AVAudioEnvironmentNode instance, the system may only support a subset of the rendering algorithms. You can retrieve an array of valid rendering algorithms by calling the applicableRenderingAlgorithms function of the AVAudioEnvironmentNode instance.

The default rendering algorithm is AVAudio3DMixingRenderingAlgorithm.equalPowerPanning. Only the AVAudioEnvironmentNode class implements this property.

## See Also

### Getting and Setting the Rendering Algorithm

enum AVAudio3DMixingRenderingAlgorithm

The types of rendering algorithms available per input bus of the environment node.

