

- Core Telephony
- CTTelephonyNetworkInfoDelegate
-  dataServiceIdentifierDidChange(\_:) 

Instance Method

# dataServiceIdentifierDidChange(\_:)

Informs the delegate when the identifier changes for the service that’s currently providing data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func dataServiceIdentifierDidChange(_ identifier: String)
```

## Parameters 

`identifier`  

The identifier of the service that’s currently providing data. Use this identifier as the key in serviceCurrentRadioAccessTechnology to get the value of the new radio access technology for the service.

