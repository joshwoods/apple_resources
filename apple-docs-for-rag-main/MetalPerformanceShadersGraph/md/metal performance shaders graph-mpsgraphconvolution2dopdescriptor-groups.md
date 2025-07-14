

- Metal Performance Shaders Graph
- MPSGraphConvolution2DOpDescriptor
-  groups 

Instance Property

# groups

The number of partitions of the input and output channels.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var groups: Int { get set }
```

## Discussion

The convolution operation divides input and output channels in `groups` partitions. input channels in a group or partition are only connected to output channels in corresponding group. Number of weights the convolution needs is `outputFeatureChannels x inputFeatureChannels/groups x kernelWidth x kernelHeight`

