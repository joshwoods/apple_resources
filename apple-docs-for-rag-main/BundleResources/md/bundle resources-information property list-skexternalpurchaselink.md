

- Bundle Resources
- Information Property List
-  SKExternalPurchaseLink 

Property List Key

# SKExternalPurchaseLink

A dictionary that contains URLs to websites where people using your app can make external purchases for supported regions.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

## Details 

Type  

object

## Properties

`Any Key`

`string`

## Discussion

Use this information property list key if your app has the com.apple.developer.storekit.external-purchase-link entitlement and your app has a minimum OS version prior to iOS 17.5, macOS 14.5, watchOS 10.5, tvOS 17.5, or visionOS 1.2. Otherwise, use the SKExternalPurchaseMultiLink property list key to provide multiple URLs for country codes that allow multiple links.

The keys for this dictionary are lowercased ISO 3166-1 alpha-2 country codes. Valid country codes include those for the European Union: Austria (`at`), Belgium (`be`), Bulgaria (`bg`), Croatia (`hr`), Cyprus (`cy`), Czechia (`cz`), Denmark (`dk`), Estonia (`ee`), Finland (`fi`), France (`fr`), Germany (`de`), Greece (`gr`), Hungary (`hu`), Ireland (`ie`), Italy (`it`), Latvia (`lv`), Lithuania (`lt`), Luxembourg (`lu`), Malta (`mt`), Netherlands (`nl`), Poland (`pl`), Portugal (`pt`), Romania (`ro`), Slovakia (`sk`), Slovenia (`si`), Spain (`es`), Sweden (`se`); and Iceland (`is`), Norway (`no`), Russia (`ru`), and United States (`us`).

Include one key entry for each country code where your app supports an external purchase link. Provide a destination URL (link to your website) for your app to open when the country code in the key matches the device’s App Store storefront. If you support multiple country codes, you may provide the same or different destination URLs for each country code.

Important

At all times, the destination URLs that you provide in the property list key must match the values in your app binary that you submit to App Review.

Make sure the destination URL meets all of the following conditions:

- Uses the HTTPS scheme

- Forms a valid, absolute URL

- Contains no query parameters

- Contains 1,000 or fewer ASCII characters.

The following code example shows a property list entry with a single country code key, for the Netherlands (`nl`). Replace the string “`https://example.com`” below with your link:

```

    SKExternalPurchaseLink

        nl
        https://example.com

```

The following code example shows a property list entry with keys for more than one country code. Replace the “`https://example.com`” strings with your links:

```

    SKExternalPurchaseLink

        at
        https://ex1.example.com
        nl
        https://ex2.example.com
        it
        https://ex2.example.com

```

For more information, see External Purchase.

## See Also

### StoreKit

SKAdNetworkItems

An array of dictionaries containing a list of ad network IDs.

SKExternalLinkAccount

A dictionary that contains localized URLs to an external website for account creation or management.

SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

SKExternalPurchaseCustomLinkRegions

An array of country code strings that indicate the regions where your app supports custom links for external purchases.

SKExternalPurchaseMultiLink

A dictionary that contains an array of URLs to websites where people using your app can make external purchases.

SKIncludeConsumableInAppPurchaseHistory

A Boolean value that determines whether StoreKit includes finished consumable In-App Purchases in transaction information.

