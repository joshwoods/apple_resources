

- FSKit
- FSContainerIdentifier
-  volumeIdentifier 

Instance Property

# volumeIdentifier

The volume identifier associated with the container.

macOS 15.4+

``` source
@NSCopying
var volumeIdentifier: FSVolume.Identifier { get }
```

## Discussion

For unary file systems, the volume identifier is the same as the container identifier.

