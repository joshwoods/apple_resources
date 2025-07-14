

- Shared With You
- SWHighlightCenter
-  getSignedIdentityProof(for:using:completionHandler:) 

Instance Method

# getSignedIdentityProof(for:using:completionHandler:)

Signs passed-in data with the local device’s private key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func getSignedIdentityProof(
    for collaborationHighlight: SWCollaborationHighlight,
    using data: Data,
    completionHandler: @escaping (SWPerson.SignedIdentityProof?, (any Error)?) -> Void
)
```

``` source
func signedIdentityProof(
    for collaborationHighlight: SWCollaborationHighlight,
    using data: Data
) async throws -> SWPerson.SignedIdentityProof
```

## Parameters 

`collaborationHighlight`  

The collaboration highlight that corresponds to the `data`.

`data`  

The `NSData` that the system signs.

`completionHandler`  

Returns the signed data along with proof of inclusion for the Merkle tree if signing succeeds, otherwise an error. The system invokes the completion handler on the main thread.

## Mentioned in 

Adding custom collaboration to your app

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func signedIdentityProof(for collaborationHighlight: SWCollaborationHighlight, using data: Data) async throws -> SWPerson.SignedIdentityProof
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

When a collaboration message is sent, the system sends it individually to each of a person’s devices. Messages identifies each device using a cryptographic public key. Since the goal is to allow access only on this set of devices, the root hash is derived from the set of public keys registered to each recipient.

The root hash is the root node of a data structure called a Merkle tree. A Merkle tree is a binary tree that is built by performing a sequence of hashing operations. In order to derive an identity for the user based on their public keys, the keys are used as the leaves of this tree. The hashing algorithm used in the Merkle tree ensures that the root node can only be computed from that set of keys.

Related Sessions from WWDC22

Session 10093: Integrate your custom collaboration app with Messages

## See Also

### Retrieving collaboration highlights

class var isSystemCollaborationSupportAvailable: Bool

A Boolean value that represents full support for Messages collaboration features.

func collaborationHighlight(forIdentifier: SWCollaborationIdentifier) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified collaboration identifier.

func collaborationHighlight(forIdentifier: String) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified identifier string.

func getCollaborationHighlight(for: URL, completionHandler: (SWCollaborationHighlight?, (any Error)?) -> Void)

Returns a collaboration highlight for a specified URL.

func getHighlightFor(URL, completionHandler: (SWHighlight?, (any Error)?) -> Void)

Returns a highlight for a specified URL.

