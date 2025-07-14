

- Network Extension
- NWPath
-  isEqual(to:) Deprecated

Instance Method

# isEqual(to:)

Comparison method for NWPath objects.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func isEqual(to path: NWPath) -> Bool
```

Deprecated

Use the nw_path_is_equal(_:_:) function from the Network framework instead.

## Parameters 

`path`  

Another NWPath object to compare.

## Discussion

Returns true if the objects are equal, false otherwise. If two NWPath objects are equal, this means that the underlying network configuration (routes, interfaces, address, etc.) are the same between them.

