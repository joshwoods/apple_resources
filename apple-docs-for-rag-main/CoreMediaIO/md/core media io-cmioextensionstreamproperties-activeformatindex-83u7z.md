

- Core Media I/O
- CMIOExtensionStreamProperties
-  activeFormatIndex 

Instance Property

# activeFormatIndex

The index of the active format.

Mac Catalyst 15.4+macOS 12.3+Xcode 13.0+

``` source
@nonobjc
var activeFormatIndex: Int? { get set }
```

## Discussion

This value represents the index of the active format in the source’s formats array.

The key for this property is streamActiveFormatIndex.

## See Also

### Configuring Source Properties

var frameDuration: CMTime?

The duration of the frame.

var maxFrameDuration: CMTime?

The maximum duration of a frame.

