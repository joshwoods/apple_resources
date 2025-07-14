

- AdAttributionKit
-  Configuring a publisher app 

Article

# Configuring a publisher app

Set up a publisher app to participate in ad campaigns.

## Overview

A *publisher app* is an app that participates in ad campaigns by displaying ads that an ad network signs. To participate in install validation, the publisher app needs to include ad network IDs in its `Info.plist` file. Ad networks are responsible for publishing or providing their ad network IDs to developers.

Only ads from ad networks that have an entry in the app’s Info.plist file are eligible for install validation. To work with multiple ad networks, include each of the ad network IDs in the publisher app’s Info.plist file, as follows:

1.  Select Info.plist in the Project navigator in Xcode.

2.  Click the Add button (+) beside a key in the property list editor and press Return.

3.  Type the key name `AdNetworkIdentifiers`.

4.  Choose Array from the pop-up menu in the Type column.

5.  Create string values for each ad network ID.

Important

Lowercase the ad network ID string; otherwise, the system doesn’t recognize it as a valid network.

The following example shows an array with two strings that represent the example ad network IDs `"f2d92a.adattributionkit"` and `"2jida.adattributionkit"`:

```
"AdNetworkIdentifiers": [
  "f2d92a.adattributionkit",
  "2jida.adattributionkit"
]```

For more information about property lists, see [Edit property lists](https://help.apple.com/xcode/mac/current/#/dev3f399a2a6).
```

## See Also

### Ad network registration and configuration

Registering an ad network

Use the AdAttributionKit APIs for your ad campaigns after registering your ad network with Apple.

Configuring an advertised app

Prepare an advertised app to participate in ad campaigns.

