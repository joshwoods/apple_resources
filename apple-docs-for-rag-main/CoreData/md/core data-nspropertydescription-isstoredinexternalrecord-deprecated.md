

- Core Data
- NSPropertyDescription
-  isStoredInExternalRecord Deprecated

Instance Property

# isStoredInExternalRecord

A Boolean value that indicates whether to write the property’s data in an external record file that corresponds to the managed object.

iOS 3.0–11.0DeprecatediPadOS 3.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.13DeprecatedtvOSDeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
var isStoredInExternalRecord: Bool { get set }
```

Deprecated

Spotlight integration is deprecated. Use CoreSpotlight integration instead.

## Discussion

true if the property data should be written out in an external record file corresponding to the managed object, otherwise false. For additional information, see Core Data Spotlight Integration Programming Guide.

### Special Considerations

This property has no effect on iOS.

## See Also

### Specifying Spotlight Support

var isIndexedBySpotlight: Bool

A Boolean value that indicates whether Core Data adds the property’s value to the Core Spotlight index.

