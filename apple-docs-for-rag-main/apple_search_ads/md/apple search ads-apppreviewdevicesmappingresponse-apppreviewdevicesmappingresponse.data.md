

- Apple Search Ads
- AppPreviewDevicesMappingResponse
-  AppPreviewDevicesMappingResponse.Data 

Object

# AppPreviewDevicesMappingResponse.Data

The app preview device mapping to display name and size mapping.

Search Ads 2.0.9+

``` source
object AppPreviewDevicesMappingResponse.Data
```

## Properties

`Any Key`

`string`

A map of app preview device sizes. The key is the identifier and the value is the display name. You can also use this to define the supported fallback devices if mapping isn’t available.

```
{
  "ipadPro": "iPad 12.9",
  "iphone6+": "iPhone 5.5",
  "iphone_5_8": "iPhone 5.8",
  "iphone5": "iPhone 4",
  "iphone6": "iPhone 4.7",
  "ipadPro_2018": "iPad 11",
  "ipad": "iPad 9.7",
  "iphone_6_5": "iPhone 6.5",
  "ipad_10_5": "iPad 10.5"
}
```

