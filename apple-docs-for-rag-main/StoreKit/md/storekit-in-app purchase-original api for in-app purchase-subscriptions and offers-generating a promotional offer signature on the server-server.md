

- StoreKit
- In-App Purchase
- Original API for In-App Purchase
- Subscriptions and offers
-  Generating a Promotional Offer Signature on the Server 

Sample Code

# Generating a Promotional Offer Signature on the Server

Generate a signature using your private key and lightweight cryptography libraries.

Download

## Overview

Note

This sample code project is associated with WWDC 2019 session 305: Subscription Offers Best Practices.

This sample code is a simple server written using JavaScript and Node.js. It demonstrates how to generate a signature for promotional offers. The sample demonstrates:

- Receiving a request.

- Generating a cryptographic signature using your private key.

- Sending back a response with the signature.

All of the work is done in `routes/index.js`. You set up environment variables for your key ID and your private key in the `start-server` file.

### Configure the Sample Code Project

1.  Install the latest stable version of Node.js.

2.  Open Terminal.app and navigate to the sample code directory.

3.  Run `npm install` from the command line, and make sure it completes successfully.

4.  The `start-server` file contains a key ID and private key PEM string. The values provided in the sample are for example purposes only and will not generate signatures that are valid for your apps. You can optionally open `start-server` with a text editor and replace the example key ID and private key PEM string with your own key ID and private key PEM string that you received from App Store Connect.

### Run a Test on Your Local Server

To test the code on your local machine, from the command line:

- Navigate to the sample code source folder and run `./start-server` from the command line. The server is now running locally and is ready to accept connections on port 3000.

- Open another terminal window and use the `curl` command to send a request. This example command uses the same data listed in the JSON example below:

```
curl -X GET -H "Content-type: application/json" -d '{"appBundleID": "com.example.yourapp", "productIdentifier": "com.example.yoursubscription", "offerID": "your_offer_id", "applicationUsername": "8E3DC5F16E13537ADB45FB0F980ACDB6B55839870DBCE7E346E1826F5B0296CA"}' http://127.0.0.1:3000/offer
```

You will get a response that includes the signature.

### Send a Request

To run this sample code, send a request to this URL: `GET http:///offer`, where `` is the domain name or IP address of the server this sample code is running on.

The request must have a `Content-type` header of `application/json`, and JSON body data with the following format:

```
{
    "appBundleID": "com.example.yourapp",
    "productIdentifier": "com.example.yoursubscription",
    "offerID": "your_offer_id",
    "applicationUsername": "8E3DC5F16E13537ADB45FB0F980ACDB6B55839870DBCE7E346E1826F5B0296CA"
}
```

## See Also

### Promotional offers

Setting up promotional offers

Generate a key and configure offers for auto-renewable subscriptions in App Store Connect.

Implementing promotional offers in your app

Offer discounted pricing for auto-renewable subscription products to eligible subscribers.

Generating a signature for promotional offers

Create a signature to validate a promotional offer using your private key.

class SKPaymentDiscount

The signed discount to apply to a payment.

Deprecated

