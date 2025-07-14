

- App Store Connect API
- Alternative Marketplaces and Web Distribution
- Alternative Distribution Packages
-  Creating alternative distribution packages 

Article

# Creating alternative distribution packages

Create distribution packages for your apps that you distribute on alternative marketplaces or on the web.

## Overview

Use alternative distribution package (ADP) endpoints to create new packages and read information about package versions, variants, and deltas.

### Determing eligibilty to create alternative distribution packages

Your app is eligible for an alternative distribution package if all of the following are true:

- You accept the Alternative Terms Addendum for Apps in the EU. For more information, see Update on apps distributed in the European Union.

- Your app is an iOS, iPadOS app, or targets both platforms.

- Your app version uses the iOS or iPadOS 16.1 SDK or later.

- Your App Review approved app version is in `Pending Developer Release, Pending Apple Release,` or `Ready for Distribution.`

Additionally, one of these must be true:

- Your app is connected to an alternative marketplace. For more information, see Manage distribution on an alternative marketplace.

- Your app is an alternative marketplace. For more information, see Configuring alternative marketplaces and alternative marketplace apps.

- Your app is a web distribution app. For more infomation, see Configuring apps for web distribution.

Note

Alternative marketpaces, apps distributed by alternative marketplaces, and web distribution apps all use alternative distribution packages. Web distribution apps do not use Notifications or Marketplace Search Configurations.\`\`

### Create and manage alternative distribution packages for an alternative marketplace

As an app developer for alternative marketplaces, when you add an app to a marketplace integration for distribution on a specific marketplace, you can opt-in to notifications. These notifications alert the marketplace when there are certain changes to your apps — for example, when a new alternative distribution package is generated. For more information on managing notifications, see Notifications.

After your app is approved by App Review, and after you add it to a marketplace integration in App Store Connect, you need to create the alternative distribution package. Start by finding the app Apple ID for your app by using List Apps and searching the resulting pages for the name of the app you want. In the response, make note of the `id` of that app, which appears in the following format:

```
{
  "data" : [
    {
      "type" : "apps",
      "id" : "6448401697",
      ...
```

You can also find the app Apple ID by going to App Store Connect \> My Apps \> Select an app \> App Information \> Apple ID. Next, look up the `appStoreVersion` by calling List All App Store Versions for an App using the app Apple ID. Then, call Create an alternative distribution package using the `data.relationships.appStoreVersion.id` from the previous response. Use the sample payload below as a guide:

```
{
  "data": {
    "type": "alternativeDistributionPackages",
    "relationships": {
      "appStoreVersion": {
        "data": {
          "type": "appStoreVersions",
          "id": "76931be7-95c6-470d-ace0-f3e208fd4b00"
        }
      }
    }
  }
}
```

If you opt-in to notifications, and the associated marketplace has set up webhooks with the Add a marketplace webhook configuration endpoint, the marketplace is notified that a new alternative distribution package is available. If you did not opt-in, you’ll need to provide the alternative distribution package ID to the marketplace.

If you manage an alternative marketplace, you can get the alternative distribution package ID either from a notification from the webhooks API or manually from the app developer. A marketplace can’t generate alternative distribution packages on behalf of the app developer. The marketplace developer uses the App Store Connect API key associated with the marketplace provider’s account to download ADPs.

To learn more about server-side processing of marketplace webhooks, see Processing alternative app marketplace notifications.

### Create and manage alternative distribution packages for web distribution apps

After your web distribution app is approved by App Review, you need to create the alternative distribution package. Start by finding the app Apple ID for your app by using List Apps and searching the resulting pages for the name of the app you want. In the response, make note of the `id` of that app, which appears in the following format:

```
{
  "data" : [
    {
      "type" : "apps",
      "id" : "6448401697",
      ...
```

You can also find the app Apple ID by going to App Store Connect \> My Apps \> Select an app \> App Information \> Apple ID. Next, look up the `appStoreVersion` by calling List All App Store Versions for an App using the app Apple ID. Then, call Create an alternative distribution package using the `data.relationships.appStoreVersion.id` from the previous response. Use the sample payload below as a guide:

```
{
  "data": {
    "type": "alternativeDistributionPackages",
    "relationships": {
      "appStoreVersion": {
        "data": {
          "type": "appStoreVersions",
          "id": "76931be7-95c6-470d-ace0-f3e208fd4b00"
        }
      }
    }
  }
}
```

To learn more about next steps for your web distribution app, see Installing your app from your website.

### Select the most recent distribution package

Only one alternative distribution package can exist for an `appStoreVersion.` It’s possible that you might have multiple versions of an alternative distribution package. To ensure you’re selecting the most recent `alternativeDistributionPackageVersion` when there are multiple versions available, use `filter[state]=COMPLETED` when calling the Read version information for an alternative distribution package endpoint.

## See Also

### Creating and reading distribution packages

Read alternative distribution package information

Get information about a specific alternative distribution package.

Create an alternative distribution package

Create an alternative distribution package for an app store version.

Read an App Store version’s alternative distribution package

Read the alternative distribution package for a specific App Store version.

Read version information for an alternative distribution package

Get version detail information about a specific alternative distribution package.

