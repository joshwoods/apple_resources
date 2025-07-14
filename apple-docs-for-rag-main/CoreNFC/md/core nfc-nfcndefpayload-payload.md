

- Core NFC
- NFCNDEFPayload
-  payload 

Instance Property

# payload

The payload, as defined by the NDEF specification.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var payload: Data { get set }
```

## See Also

### Getting Information About a Payload Record

var identifier: Data

The identifier of the payload, as defined by the NDEF specification.

var type: Data

The type of the payload, as defined by the NDEF specification.

var typeNameFormat: NFCTypeNameFormat

The Type Name Format field of the payload, as defined by the NDEF specification.

enum NFCTypeNameFormat

The Type Name Format values that specify the content type for the payload data in an NFC NDEF message.

