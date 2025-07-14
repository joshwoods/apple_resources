

- Core NFC
- NFCISO7816APDU
-  expectedResponseLength 

Instance Property

# expectedResponseLength

The expected response data length (Le) in bytes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var expectedResponseLength: Int { get }
```

## Discussion

Setting expectedResponseLength with a value less than 0 means the Le field is absent.

