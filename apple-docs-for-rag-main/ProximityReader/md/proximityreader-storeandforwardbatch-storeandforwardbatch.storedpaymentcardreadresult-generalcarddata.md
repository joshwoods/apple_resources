

- ProximityReader
- StoreAndForwardBatch
- StoreAndForwardBatch.StoredPaymentCardReadResult
-  generalCardData 

Instance Property

# generalCardData

A Base64-encoded string that contains general cardholder and terminal data in tag-length-value (TLV) format.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
let generalCardData: String
```

## Discussion

The content of this field is determined by your payment service provider. This field can contain both card tags and terminal tags.

