

- App Store Connect API
- App
-  App.Attributes 

Object

# App.Attributes

Attributes that describe an Apps resource.

App Store Connect API 1.0+

``` source
object App.Attributes
```

## Properties

`bundleId`

`string`

The bundle ID for your app. This ID must match the one you use in Xcode. The bundle ID cannot be changed after you upload your first build.

`name`

`string`

The name of your app as it will appear in the App Store. The maximum length is 30 characters.

`primaryLocale`

`string`

The primary locale for your app. If localized app information isn’t available in an App Store territory, the information from your primary language is used instead.

`sku`

`string`

A unique ID for your app that is not visible on the App Store.

`contentRightsDeclaration`

`string`

Possible Values: `DOES_NOT_USE_THIRD_PARTY_CONTENT, USES_THIRD_PARTY_CONTENT`

`isOrEverWasMadeForKids`

`boolean`

`subscriptionStatusUrl`

`uri`

`subscriptionStatusUrlForSandbox`

`uri`

`subscriptionStatusUrlVersion`

SubscriptionStatusUrlVersion

`subscriptionStatusUrlVersionForSandbox`

SubscriptionStatusUrlVersion

`streamlinedPurchasingEnabled`

`boolean`

## Mentioned in 

App Store Connect API 1.6 release notes

## See Also

### Related Documentation

Apps

Manage your apps in App Store Connect.

### Objects

object App.Relationships

The relationships you included in the request and those on which you can operate.

