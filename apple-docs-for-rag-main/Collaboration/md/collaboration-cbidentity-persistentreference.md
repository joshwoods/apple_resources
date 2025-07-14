

- Collaboration
- CBIdentity
-  persistentReference 

Instance Property

# persistentReference

Returns a persistent reference to store a reference to an identity.

macOS 10.5+

``` source
var persistentReference: Data? { get }
```

## Return Value

A data object that uniquely references an identity.

## Discussion

A persistent reference data object is an object generated from an identity. Persistent data objects can be written to and read from a file, making them extremely useful for storing identities in an ACL.

