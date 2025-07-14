

- Wallet Passes
-  Return a Personalized Pass 

Web Service Endpoint

# Return a Personalized Pass

Create and sign a personalized pass, and send it to a device.

iOS 10.0+iPadOS 6.0+watchOS 2.0+

## URL

``` source
POST https://yourpasshost.example.com/v1/passes/{passTypeIdentifier}/{serialNumber}/personalize
```

## Path Parameters

`passTypeIdentifier`

`string`

 (Required) 

The pass type identifier of the pass. This value corresponds to the value of the `passTypeIdentifier` key of the pass.

`serialNumber`

`string`

 (Required) 

The serial number of the pass. This value corresponds to the `serialNumber` key of the pass.

## HTTP Body

PersonalizationDictionary

An object that contains the personalization information for the pass.

Content-Type: application/json

## Response Codes

` 200 ``OK`

`OK`

The request is successful and returns a signed personalization token.

Content-Type: application/octet-stream

## See Also

### Personalized Passes

object PersonalizationDictionary

An object that contains the information you use to personalize a pass.

