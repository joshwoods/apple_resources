

- User Notifications
-  Sending push notifications using command-line tools 

Article

# Sending push notifications using command-line tools

Use basic macOS command-line tools to send push notifications to Apple Push Notification service (APNs).

## Overview

Testing your APNs connection and configuration by writing a test app can take time. The command-line tools described below provide a quick way to test your setup with APNs in a nonproduction-quality test suite or app.

Before you begin, verify that:

- Your target device is unlocked and connected to the internet.

- Your app is open and in the foreground.

### Send a push notification using a certificate

To send a push notification using a certificate, you’ll need:

- A DER-encoded certificate from WWDR to connect to the APNs sandbox. For details on how to set up certificate-based trust with APNs, refer to Establishing a certificate-based connection to APNs.

- The PEM-encoded private key, without a password, used to generate the above certificate. The Keychain app generates the private key when you create a certificate signing request (CSR). To learn more, refer to Create a certificate signing request.

- Your App ID. To learn more about App IDs, refer to Register an App ID.

Start by launching the Terminal app in the most recent macOS version. Then set these shell variables:

```
```

Whether you’re testing a device or a broadcast push notification determines the next set of variables to include.

### Send a device push notification using a certificate

To send a device push notification using a certificate, you’ll need:

- The device token from your app, as a hexadecimal-encoded ASCII string. To learn more about device tokens, refer to Registering your app with APNs.

In the Terminal app in the most recent macOS version, set these additional shell variables:

```
```

Test that you can use your certificate to connect to APNs using this command:

```
```

Then send a push notification using this command:

```
```

The result is an HTTP status of 200 (request succeeded). A notification with the text “test” appears on your destination device.

### Send a broadcast push notification using a certificate

To send a broadcast push notification using a certificate, you’ll need:

- The channel ID you’re using for the broadcast, as a base64-encoded string. For more information about creating a channel, refer to Sending channel management requests to APNs.

- Ensure the Live Activity is active on the device.

In the Terminal app in the most recent macOS version, set these additional shell variables:

```
```

Test that you can use your certificate to connect to APNs using this command:

```
```

Then send a push notification using this command:

```
```

The result is an HTTP status of 200 (request succeeded). Update the data in the curl command based on your Live Activity.

### Send a push notification using a JSON web token (JWT)

To send a push notification using a JWT, you’ll need:

- Your Team ID. For more information, refer to Locate your Team ID.

- Your key identifier for APNs. For more information, refer to Get a key identifier.

- The PEM-encoded private key, without a password, associated with the above key identifier. To learn more about downloading keys, refer to Revoke, edit, and download keys.

- Your App ID. To learn more about App IDs, refer to Register an App ID.

Start by launching the Terminal app in the most recent macOS version. Then set these shell variables:

```
```

Whether you’re testing a device or a broadcast push notification determines the next set of variables to include.

### Send a device push notification using a JWT

To send a device push notification using a JWT, you’ll need:

- The device token from your app, as a hexadecimal-encoded ASCII string. To learn more about device tokens, refer to Registering your app with APNs.

In the Terminal app, set these additional shell variables:

```
```

Test that you can connect to APNs using this command:

```
```

Set these additional shell variables just before sending a push notification:

```
```

Send the push notification using this command:

```
```

The result is an HTTP status of 200 (request succeeded). A notification with the text “test” appears on your destination device.

### Send a broadcast push notification using a JWT

To send a broadcast push notification using a JWT, you’ll need:

- The channel ID you’re using for the broadcast, as a base64-encoded string. For more information about creating a channel, refer to Sending channel management requests to APNs.

- Ensure the Live Activity is active on the device.

In the Terminal app in the most recent macOS version, set these additional shell variables:

```
```

Test that you can use your certificate to connect to APNs using this command:

```
```

Set these additional shell variables just before sending a push notification:

```
```

Then send a push notification using this command:

```
```

The result is an HTTP status of 200 (request succeeded). Update the data in the curl command based on your Live Activity.

## See Also

### Remote notifications

Setting up a remote notification server

Generate notifications and push them to user devices.

Testing notifications using the Push Notification Console

Send test notifications and access delivery logs to test your app’s integration with Apple Push Notification service (APNs).

