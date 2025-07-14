

- Bundle Resources
- Information Property List
-  SKExternalPurchaseCustomLinkRegions 

Property List Key

# SKExternalPurchaseCustomLinkRegions

An array of country code strings that indicate the regions where your app supports custom links for external purchases.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+tvOS 18.1+visionOS 2.1+watchOS 11.1+

## Details 

Type  

array of strings

## Discussion

Use this information property list key if your app has the com.apple.developer.storekit.external-purchase-link entitlement and uses the ExternalPurchaseCustomLink API.

Include an entry for each country code where your app supports custom links for external purchases.

Valid country codes include the European Union: Austria (`at`), Belgium (`be`), Bulgaria (`bg`), Croatia (`hr`), Cyprus (`cy`), Czechia (`cz`), Denmark (`dk`), Estonia (`ee`), Finland (`fi`), France (`fr`), Germany (`de`), Greece (`gr`), Hungary (`hu`), Ireland (`ie`), Italy (`it`), Latvia (`lv`), Lithuania (`lt`), Luxembourg (`lu`), Malta (`mt`), Netherlands (`nl`), Poland (`pl`), Portugal (`pt`), Romania (`ro`), Slovakia (`sk`), Slovenia (`si`), Spain (`es`), Sweden (`se`).

## See Also

### StoreKit

SKAdNetworkItems

An array of dictionaries containing a list of ad network IDs.

SKExternalLinkAccount

A dictionary that contains localized URLs to an external website for account creation or management.

SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

SKExternalPurchaseLink

A dictionary that contains URLs to websites where people using your app can make external purchases for supported regions.

SKExternalPurchaseMultiLink

A dictionary that contains an array of URLs to websites where people using your app can make external purchases.

SKIncludeConsumableInAppPurchaseHistory

A Boolean value that determines whether StoreKit includes finished consumable In-App Purchases in transaction information.

