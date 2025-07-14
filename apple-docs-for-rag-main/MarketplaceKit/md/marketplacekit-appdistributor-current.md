

- MarketplaceKit
- AppDistributor
-  current 

Type Property

# current

The source from which the app installs.

iOS 17.4+iPadOS 17.4+Mac CatalystmacOS 15.0+

``` source
static var current: AppDistributor { get async throws }
```

## Mentioned in 

Distributing your app on an alternative app marketplace

Distributing your app from your website

## Discussion

iOS sets the value of this property to an AppDistributor enumeration case that describes the running app’s manner of distribution. If your app installs from more than one source, you can implement conditional code to do something different based on the value of this property at runtime, for example, your app can display a different graphic.

For more information, see Distributing your app on an alternative app marketplace.

