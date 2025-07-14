

- ManagedSettings
- AppStoreSettings
-  maximumRating 

Type Property

# maximumRating

The metadata associated with the maximum app rating setting.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let maximumRating: BoundedSettingMetadata
```

## Discussion

Use `maximumRating` to access the metadata for maximumRating. The default value is `1000` and the bounds are `0...2000`.

## See Also

### Setting an App Rating Limit

var maximumRating: Int?

The maximum app rating the user can download.

