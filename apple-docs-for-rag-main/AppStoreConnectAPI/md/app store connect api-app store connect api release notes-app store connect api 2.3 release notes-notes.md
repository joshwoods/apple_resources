

- App Store Connect API
- App Store Connect API Release Notes
-  App Store Connect API 2.3 release notes 

Article

# App Store Connect API 2.3 release notes

Update your server-side code to use new features, and test your code against API changes.

### New features

- Getting an app’s price points and List All Price Points for an In-App Purchase now support 900 price points.

- List app price point equalizations allows for setting equalized prices.

- Getting and managing an app’s price schedules and In-App purchase price schedules support automatic prices, manual prices, and base territory configuration.

- Getting and managing an app’s availability, In-app purchase availability and Subscription availability supports configuring availabilty for apps, in-app purchases, and subscriptions.

### Deprecations

- The `List all price points for an app V1` endpoint is now deprecated and replaced with List all price points for an app.

- The `List all prices for an app` endpoint is now deprecated and replaced with Read price schedule information for an app.

- The `List all available territories for an app` endpoint is now deprecated and replaced with `GET-v1-appAvailabilities-{id}`.

- The `AppPricePointV2` object deprecated and replaced with AppPricePointV3.

- The `List all price points for an app V1` endpoint is now deprecated and replaced with `List app price tiers`.

- The `Read app price tier information` endpoint is now deprecated and replaced with `Read App Price Point Information`.

Important

If you use Add a scheduled price change to an app to add a scheduled price change to your App, you can’t use `AppPriceInlineCreate` to change your App’s price.

### Note to Developers

On May 9, 2023, pricing for your existing apps and in-app purchases (excluding auto-renewable subscriptions) will be updated across all 175 storefronts to be equalized to your base country or region using publicly available exchange rate information. If you don’t specify a base country or region, Apple will use your current price in the United States as the basis to provide comparable prices in other countries or regions. Learn more about app or in-app purchase pricing.

## See Also

### Versions

App Store Connect API 3.8 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.7 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.6 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.5 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.4 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.3 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.2 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.1 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.0 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.4 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.2 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.1 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.0 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 1.8 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 1.7 release notes

Update your server-side code to use new features, and test your code against API changes.

