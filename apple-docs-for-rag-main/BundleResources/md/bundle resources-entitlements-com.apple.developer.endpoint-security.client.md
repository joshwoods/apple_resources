

- Bundle Resources
- Entitlements
-  com.apple.developer.endpoint-security.client 

Property List Key

# com.apple.developer.endpoint-security.client

The entitlement required to monitor system events for potentially malicious activity.

macOS 10.15+

## Details 

Type  

boolean

## Discussion

You must request this entitlement from Apple. For information about how to request the entitlement, see System Extensions and DriverKit.

If your app or extension lacks this requirement, es_new_client(_:_:) fails with the result ES_NEW_CLIENT_RESULT_ERR_NOT_ENTITLED.

