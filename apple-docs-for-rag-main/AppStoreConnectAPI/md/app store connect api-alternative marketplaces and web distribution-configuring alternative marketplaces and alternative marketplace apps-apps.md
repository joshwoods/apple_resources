

- App Store Connect API
- Alternative Marketplaces and Web Distribution
-  Configuring alternative marketplaces and alternative marketplace apps 

Article

# Configuring alternative marketplaces and alternative marketplace apps

Establish a connection between a marketplace and a marketplace app and configure marketplace settings.

## Overview

Use the Alternative Marketplaces and Web distribution API to create and configure alternative marketplaces. Once you create a marketplace app record in App Store Connect, you can add configurations for:

- Alternative distribution domains

- Search detail URLs

- Webhook endpoint URLs

### Connect your marketplace to the apps it distributes

Begin creating the connection between your alternative marketplace and the apps it distributes, by making a new app record, or making a new one in App Store Connect. Next, create a public and private key pair to associate with your marketplace. For more information, see Creating keys and establishing alternative marketplace connections.

Next, you upload the public key along with your marketplace’s app Apple ID by using Add an alternative distribution key.

Next, you create a signed JSON web token (JWT) for the app devleoper to upload to App Store Connect. The JWT requires your private key, the app developer’s Developer ID, and your marketplace’s app Apple ID.

While uploading the JWT, the app developer selects the apps they want to associate with your marketplace. At this point, the app developer can also enable notifications which are delivered by webhooks. For more information about notifications and webhooks, see Notifications.

Note

Apps can be distributed on App Store, an alternative marketplace or both. To learn more, see AppStoreVersionUpdateRequest.Data.Attributes, specifically `reviewType` and Modify an App Store Version.

### Set up the marketplace

You need to configure several parts of your alternative marketplace so it can function properly and interact with Apple resources. You need to:

- Configure Add a marketplace webhook configuration with the server `endpointUrl,` so it listens for new notifications. For more information, see Notifications.

- Add an alternative distribution domain to represent your marketplace app’s base web domain, from which all traffic must flow. This domain serves your marketplace app and all other apps on individual pages on your marketplace.

- Set up your marketplace search detail so Apple can crawl your sitemap and include your apps in Spotlight search, using Add a marketplace search detail URL. To learn more, see Building a searchable catalog for your marketplace app for inclusion in Spotlight.

Next, you need to process alternative distribution packages. For more information, see Processing alternative app marketplace notifications.

Next, you need to obtain the alternative distribution package ID; follow these steps based on whether the app you distribute is already approved by App Review:

- If the app to be distributed on an alternative marketplace is already approved, the app developer needs to generate an alternative distribution package by using the Create an alternative distribution package endpoint.

- If the app to be distributed on an alternative marketplace is not in one of the following states (all of which are after approval by App Review): `Pending Developer Release, Pending Apple Release,` or `Ready for Distribution,` the alternative distribution package is automatically created after approval.

- Once the alternative distribution package is created, and the alternative distribution package ID is provided to the marketplace, either by the app developer or though webhooks, the marketplace can ingest and process the provided files. To learn more, see Processing alternative app marketplace notifications.

## See Also

### Essentials

Configuring apps for web distribution

Set up your app for direct installation.

