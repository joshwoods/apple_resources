

- Network Extension
- NWBonjourServiceEndpoint
-  init(name:type:domain:) Deprecated

Initializer

# init(name:type:domain:)

Create an endpoint with a Bonjour service name, type, and domain. All fields must be specified.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
convenience init(
    name: String,
    type: String,
    domain: String
)
```

Deprecated

Use the nw_endpoint_create_bonjour_service(_:_:_:) function from the Network framework instead.

## Parameters 

`name`  

The Bonjour service name.

`type`  

The Bonjour service type.

`domain`  

The Bonjour service domain.

## Return Value

The new NWBonjourServiceEndpoint object.

