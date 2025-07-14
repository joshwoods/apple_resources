

- Foundation
- XMLDocument
-  xmlData(options:) 

Instance Method

# xmlData(options:)

Returns the XML string representation of the receiver—that is, the entire document—encapsulated in a data object.

Mac Catalyst 13.0+macOS 10.0+

``` source
func xmlData(options: XMLNode.Options = []) -> Data
```

## Parameters 

`options`  

One or more options (bit-OR’d if multiple) to affect the output of the document; see Constants for the valid output options.

## Discussion

The encoding used is based on the value returned from characterEncoding.

## See Also

### Writing a Document as XML Data

var xmlData: Data

Returns the XML string representation of the receiver—that is, the entire document—encapsulated in a data object.

