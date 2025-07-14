

- AVFAudio
- AVAudioEnvironmentNode
-  applicableRenderingAlgorithms 

Instance Property

# applicableRenderingAlgorithms

An array of rendering algorithms applicable to the environment node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var applicableRenderingAlgorithms: [NSNumber] { get }
```

## Discussion

The `AVAudioEnvironmentNode` class supports several rendering algorithms for each input bus as AVAudio3DMixingRenderingAlgorithm defines.

Depending on the current output format of the environment node, this method returns an immutable array of the applicable rendering algorithms. This subset of applicable rendering algorithms is important when you configure the environment node to a multichannel output format because only a subset of the algorithms render to all of the channels.

Retrieve the applicable algorithms after a successful connection to the destination node through one of the AVAudioEngine connect methods.

## See Also

### Related Documentation

func connect(AVAudioNode, to: AVAudioNode, format: AVAudioFormat?)

Establishes a connection between two nodes.

func connect(AVAudioNode, to: AVAudioNode, fromBus: AVAudioNodeBus, toBus: AVAudioNodeBus, format: AVAudioFormat?)

Establishes a connection between two nodes, specifying the input and output busses.

