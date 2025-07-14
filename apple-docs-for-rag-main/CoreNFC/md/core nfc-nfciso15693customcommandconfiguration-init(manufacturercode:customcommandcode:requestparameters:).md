

- Core NFC
- NFCISO15693CustomCommandConfiguration
-  init(manufacturerCode:customCommandCode:requestParameters:) 

Initializer

# init(manufacturerCode:customCommandCode:requestParameters:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
init(
    manufacturerCode: Int,
    customCommandCode: Int,
    requestParameters: Data?
)
```

## Parameters 

`manufacturerCode`  

8 bits manufacturer code.

`customCommandCode`  

8 bits custom command code. Valid range is 0xA0 to 0xDF.

`requestParameters`  

Optional custom request parameters.

## Discussion

Initialize with default zero maximum retry and zero retry interval.

