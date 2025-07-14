

- Shared With You Core
- SWPerson
- SWPerson.IdentityProof
-  inclusionHashes 

Instance Property

# inclusionHashes

The hashes of missing Merkle tree nodes that can provide proof of inclusion.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var inclusionHashes: [Data] { get }
```

## Discussion

The data contains an array of SHA256 hash of the user’s combined public identities.

## See Also

### Accessing attributes

var publicKey: Data

The public key of local device.

var publicKeyIndex: Int

The index of the local public key in the Merkle tree.

