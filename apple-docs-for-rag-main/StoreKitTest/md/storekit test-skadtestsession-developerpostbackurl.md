

- StoreKit Test
- SKAdTestSession
-  developerPostbackURL 

Instance Property

# developerPostbackURL

The URL that SKAdNetwork computes to send copies of winning postbacks to the advertised app’s developer.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var developerPostbackURL: URL? { get }
```

## Discussion

Use this property to view the URL that SKAdNetwork computes to send a copy of the winning postback to the developer. This property has a valid URL only if you specify a valid URL in the NSAdvertisingAttributionReportEndpoint key in your app’s `Info.plist`. For more information, see Configuring an advertised app.

Note

The testing environment doesn’t use this URL. SKAdNetwork sends copies of winning postbacks in the production environment only.

