

- Foundation
- XMLDTDNode
-  notationName 

Instance Property

# notationName

Returns the name of the notation associated with the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var notationName: String? { get set }
```

## Return Value

The name of the notation associated with the receiver.

## Discussion

Notations are applicable to unparsed external entities, processing instructions, and some attribute values.

## See Also

### Managing DTD Identifiers

var isExternal: Bool

var publicID: String?

Returns the public identifier associated with the receiver.

var systemID: String?

Returns the system identifier associated with the receiver.

