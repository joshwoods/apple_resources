

- StoreKit
- Ad network attribution
- SKAdNetwork
-  Configuring a source app 

Article

# Configuring a source app

Set up a source app to participate in ad campaigns.

## Overview

A *source app* is an app that participates in ad campaigns by displaying ads that an ad network signs. To participate in install validation, the source app needs to include ad network IDs in its `Info.plist` file. Ad networks are responsible for publishing or providing their ad network IDs to developers.

Only ads from ad networks that have an entry in the app’s `Info.plist` file are eligible for install validation. To work with multiple ad networks, include each of the ad network IDs in the source app’s `Info.plist` file, as follows:

1.  Select `Info.plist` in the Project navigator in Xcode.

2.  Click the Add button (+) beside a key in the property list editor and press Return.

3.  Type the key name SKAdNetworkItems.

4.  Choose Array from the pop-up menu in the Type column.

Create an array that contains one dictionary for each allowed ad network, using the single key SKAdNetworkIdentifier. The string value for the key is the ad network ID.

Important

Lowercase the ad network ID string; otherwise, the system doesn’t recognize it as valid.

The following example shows an array with two dictionaries that represent the example ad network IDs `example100.skadnetwork` and `example200.skadnetwork`:

```

        SKAdNetworkIdentifier
        example100.skadnetwork

         SKAdNetworkIdentifier
         example200.skadnetwork

```

For more information about property lists, see Edit property lists.

## See Also

### Registering ad networks and configuring apps

Registering an ad network

Use the install-validation APIs for your ad campaigns after registering your ad network with Apple.

Configuring an advertised app

Prepare an advertised app to participate in ad campaigns.

SKAdNetworkItems

An array of dictionaries containing a list of ad network IDs.

NSAdvertisingAttributionReportEndpoint

The URL where Private Click Measurement and SKAdNetwork send attribution information.

