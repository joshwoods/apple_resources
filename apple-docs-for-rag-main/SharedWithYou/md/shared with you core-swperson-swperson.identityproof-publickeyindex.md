

- Shared With You Core
- SWPerson
- SWPerson.IdentityProof
-  publicKeyIndex 

Instance Property

# publicKeyIndex

The index of the local public key in the Merkle tree.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var publicKeyIndex: Int { get }
```

## Discussion

This data can be used to determine if the node is the left or the right child in the tree.

## See Also

### Accessing attributes

var inclusionHashes: [Data]

The hashes of missing Merkle tree nodes that can provide proof of inclusion.

var publicKey: Data

The public key of local device.

