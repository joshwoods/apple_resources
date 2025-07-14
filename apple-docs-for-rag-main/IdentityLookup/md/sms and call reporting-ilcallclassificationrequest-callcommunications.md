

- SMS and Call Reporting
- ILCallClassificationRequest
-  callCommunications 

Instance Property

# callCommunications

The calls the user selected to report.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
var callCommunications: [ILCallCommunication] { get }
```

## Discussion

The system sorts calls by the date received.

Currently, the user has no way to select multiple calls, so the array should only contain one call. However, in order to future-proof your app, always assume the property might contain more than one call.

