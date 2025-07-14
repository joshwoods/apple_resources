

- Core NFC
- NFCNDEFPayload
-  identifier 

Instance Property

# identifier

The identifier of the payload, as defined by the NDEF specification.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var identifier: Data { get set }
```

## See Also

### Getting Information About a Payload Record

var payload: Data

The payload, as defined by the NDEF specification.

var type: Data

The type of the payload, as defined by the NDEF specification.

var typeNameFormat: NFCTypeNameFormat

The Type Name Format field of the payload, as defined by the NDEF specification.

enum NFCTypeNameFormat

The Type Name Format values that specify the content type for the payload data in an NFC NDEF message.

