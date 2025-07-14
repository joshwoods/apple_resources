

- Bundle Resources
- Information Property List
-  SKExternalPurchase 

Property List Key

# SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

## Details 

Type  

array of strings

## Discussion

Use this information property list key if your app has the com.apple.developer.storekit.external-purchase entitlement.

To the array, add a string containing the lowercased ISO 3166-1 alpha-2 country code for each country where your app supports external purchases. The following code example shows a property list entry with two strings, for the Netherlands (`nl`) and Italy (`it`):

```

    SKExternalPurchase

        nl
        it

```

Use valid country codes for the following allowed countries or regions:

- In the European Union: Austria (`at`), Belgium (`be`), Bulgaria (`bg`), Croatia (`hr`), Cyprus (`cy`), Czechia (`cz`), Denmark (`dk`), Estonia (`ee`), Finland (`fi`), France (`fr`), Germany (`de`), Greece (`gr`), Hungary (`hu`), Ireland (`ie`), Italy (`it`), Latvia (`lv`), Lithuania (`lt`), Luxembourg (`lu`), Malta (`mt`), Netherlands (`nl`), Poland (`pl`), Portugal (`pt`), Romania (`ro`), Slovakia (`sk`), Slovenia (`si`), Spain (`es`), Sweden (`se`)

- South Korea (`kr`)

For more information, see External Purchase.

## See Also

### StoreKit

SKAdNetworkItems

An array of dictionaries containing a list of ad network IDs.

SKExternalLinkAccount

A dictionary that contains localized URLs to an external website for account creation or management.

SKExternalPurchaseCustomLinkRegions

An array of country code strings that indicate the regions where your app supports custom links for external purchases.

SKExternalPurchaseLink

A dictionary that contains URLs to websites where people using your app can make external purchases for supported regions.

SKExternalPurchaseMultiLink

A dictionary that contains an array of URLs to websites where people using your app can make external purchases.

SKIncludeConsumableInAppPurchaseHistory

A Boolean value that determines whether StoreKit includes finished consumable In-App Purchases in transaction information.

