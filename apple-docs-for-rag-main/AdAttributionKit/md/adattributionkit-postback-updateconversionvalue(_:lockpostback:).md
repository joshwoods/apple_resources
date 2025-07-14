

- AdAttributionKit
- Postback
-  updateConversionValue(\_:lockPostback:) 

Type Method

# updateConversionValue(\_:lockPostback:)

Updates a conversion value with the provided fine and coarse conversion values, and optionally locks the postback, reducing the system time to deliver a signal.

iOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
static func updateConversionValue(
    _ fineConversionValue: Int,
    lockPostback: Bool
) async throws
```

## Parameters 

`fineConversionValue`  

An integer the defines the fine conversion value.

`lockPostback`  

A Boolean value that indicates whether the system can lock the postback, reducing the system time to deliver a signal.

## Mentioned in 

Identifying the parameters in a postback

Receiving postbacks in multiple conversion windows

Understanding AdAttributionKit and SKAdNetwork interoperability

Configuring an advertised app

