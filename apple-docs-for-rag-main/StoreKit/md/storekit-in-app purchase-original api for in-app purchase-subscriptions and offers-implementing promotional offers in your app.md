

- StoreKit
- In-App Purchase
- Original API for In-App Purchase
- Subscriptions and offers
-  Implementing promotional offers in your app 

Article

# Implementing promotional offers in your app

Offer discounted pricing for auto-renewable subscription products to eligible subscribers.

## Overview

Promotional offers can be effective in winning back lapsed subscribers or retaining current subscribers. You can provide lapsed or current subscribers a limited-time offer of a discounted or free period of service for auto-renewable subscriptions on macOS, iOS, and tvOS. To implement the offers, first complete the setup on App Store Connect, including generating a private key. See Setting up promotional offers for more details.

You decide the criteria for which subscribers qualify for an offer. In your app, the details of the offers you set up in App Store Connect appear in the discounts array in SKProduct. To indicate the offer you want to give to a user, include a signed paymentDiscount in the SKMutablePayment object.

For business guidance on using promotional offers, see Auto-renewable Subscriptions > Providing Subscription Offers.

Note

If your goal is to attract new users, you can use introductory offers and promote the in-app purchase on the App Store. Users are eligible to receive only one introductory offer, but redeeming an introductory offer doesn’t affect their eligibility for a promotional offer. For more information on introductory offers, see Implementing introductory offers in your app.

### Prepare Your Offer

To present a promotional offer, first determine the subscriber’s eligibility, get the product details from the App Store, and generate a signature on your server.

#### Determine Eligibility

There are two aspects to determining a user’s eligibility for promotional offers:

- The App Store deems all customers with an existing or expired subscription in the app eligible to redeem a promotional offer. You can check whether the receipt contains any existing or expired subscription purchases to identify these current or lapsed subscribers.

- You determine any additional eligibility criteria for a specific promotional offer. Eligibility can be contingent on a wide range of business logic determined by your business needs.

Consider using the App Store server notification `DID_CHANGE_RENEWAL_STATUS` to determine eligibility. This notification is triggered by changes in a subscription’s auto-renew status. For example, you receive a notification when a subscriber disables auto-renew in Manage Subscriptions or contacts AppleCare to cancel their subscription. For more information on server notifications, see App Store Server Notifications. Your server can notify your app if the user is eligible for an offer so the app can present it to the customer.

Note

Customers can redeem promotional offers only on devices running iOS 12.2 and later, macOS 10.14.4 and later, and tvOS 12.2 and later. Consider providing messaging prompting your customer to update their OS if they try to redeem a promotional offer in your app on a device running an older OS version.

Consider also implementing DeviceCheck to keep track of devices that have previously redeemed offers. `TwoBitKit` allows you to maintain user privacy while defining parameters you use to determine eligibility.

#### Request Product Details

Once you determine that the subscriber is eligible for an offer, the next step is requesting the product details, including offers, from the App Store. To fetch the details, use SKProductsRequest with the subscription’s product identifier.

In response, the App Store returns the localized information in SKProduct. The discounts array of SKProduct contains all promotional offers you configured in App Store Connect for that product. The SKProductDiscount object contains offer details including the localized price.

You determine which offer from the discounts array to present to the user.

#### Create a Signature

A signature is a unique string that your server generates using specified parameters and your private key. You include it in the signature parameter of SKPaymentDiscount, and the App Store uses it to validate the promotional offer. The signature is time sensitive, unique per offer, and redeemable only once.

To generate the signature, send a secure request to your server. The server will need to know the applicationUsername, productIdentifier, and identifier. Your app should supply these parameters in the request if the server doesn’t already know them. See Generating a signature for promotional offers for more information.

Your server should respond with the signature string and the additional values it used to generate the signature: a `nonce`, `timestamp`, and the `keyIdentifier`. Use these values to complete the parameters in the SKPaymentDiscount object nested in the SKMutablePayment object representing the offer. If the App Store determines that the signature isn’t a match for the parameters in the payment, the transaction fails.

Tip

To minimize latency, consider generating the signature when you display the offer.

The following code example shows how to request a signature from your server and prepare the discount offer.

```
// Fetch the signature from your server to be applied to the offer.
// At this point you know the user and the product the offer is for, and which offer you want to display.
public func prepareOffer(usernameHash: String, productIdentifier: String, offerIdentifier: String, completion: (SKPaymentDiscount) -> Void) {

    // Make a secure request to your server, providing the username, product, and discount data
    // Your server will use these values to generate the signature and return it, along with the nonce, timestamp, and key identifier that it uses to generate the signature.
    YourServer.fetchOfferDetails(username: usernameHash, productIdentifier: productIdentifier, offerIdentifier: offerIdentifier, completion: { (nonce: UUID, timestamp: NSNumber, keyIdentifier: String, signature: String) in 

        // Create an SKPaymentDiscount to be used later when the user initiates the purchase
        let discountOffer = SKPaymentDiscount(identifier: offerIdentifier, keyIdentifier: keyIdentifier, nonce: nonce, signature: discountsignature, timestamp: timestamp)

        completion(discountOffer)
    })
}
```

#### Present Your Offer

You can present offers to users through various channels, such as email, but they must interact with the offer inside your app’s UI. Display the offer in your app at the time you choose, using the pricing and terms from the SKProductDiscount object. By using the details from this object, you ensure that the offer displayed to the user accurately reflects the offer you intend to give. For design guidance, see Auto-Renewable Subscriptions > Clearly Describing Subscriptions.

Present offers to eligible subscribers only, to avoid misleading or confusing users.

### Complete the Transaction

After a user chooses to buy the promotional offer, submit the payment request, verify the receipt, and unlock the offer.

#### Create a Payment Request

When the user initiates a buy of the offer in the app, send an SKMutablePayment to the App Store with the signed offer. Create an SKPaymentDiscount object that includes the signature you generated and its `identifier`, `keyIdentifier`, `nonce` (one-time use), and `timestamp` parameters. Add this object as the paymentDiscount property to the SKMutablePayment object.

Include in the SKMutablePayment object the same applicationUsername, often a unique hash of the username, that the signature contains. Add the SKMutablePayment object to the queue.

```
// An example function that makes a buy request with a promotional offer attached.
public func buyProduct(productIdentifier: SKProduct, forUser usernameHash: String, withOffer discountOffer: SKPaymentDiscount) {

    // The original product being purchased.
    let payment = SKMutablePayment(product: product)

    // You must set applicationUsername to be the same as the one used to generate the signature.
    payment.applicationUsername = usernameHash

    // Add the offer to the payment.
    payment.paymentDiscount = discountOffer

    // Add the payment to the queue for purchase.
    SKPaymentQueue.default().add(payment)
}
```

#### Notify the User of the Transaction State

Once the App Store validates the offer, it processes your payment request and generates an SKPaymentTransaction. Your app uses it to validate the transaction and unlock content accordingly.

Handle the transaction state of the payment request and notify the customer as needed. If the transaction is successful, the App Store automatically updates the app receipt with the transaction in the SKPaymentTransactionState.purchased state. Base64-encode the receipt on-device and securely send the receipt data to your server.

Note

If the transaction fails with a state of SKPaymentTransactionState.failed, you must generate a new signature and a new payment request for any further attempts to purchase the offer.

#### Verify the Receipt

As you do for all purchases, verify the receipt with the App Store by calling the verifyReceipt endpoint from your server. The App Store sends a JSON response containing information about the user’s purchase. See Validating Receipts With the App Store for more information.

When a subscriber redeems an offer, the receipt contains a promotional_offer_id in the purchase transaction. This receipt field is a string containing the offer ID that you configured in App Store Connect. You can look at past transactions in the receipt to identify the offers the customer redeemed.

#### Unlock the Service

After validating that the user has purchased the subscription product, unlock the subscription service in the app for the user. Update the customer’s eligibility criteria for offers, as needed.

When a customer redeems a promotional offer, the offer period starts at the next billing event.

- For upgrades or crossgrades to a different subscription with the same duration, the promotional offer triggers a billing event and goes into effect immediately.

- For downgrades or crossgrades to a different subscription with different durations, the promotional offer period goes into effect at the next renewal date.

- For the same subscription in an introductory offer, this promotional offer period goes into effect at the next scheduled billing event.

Once the offer period concludes, a promotional offer auto-renews at the standard price.

A user can redeem and have active only one promotional offer at a time. If the user accepts another offer before a current offer ends, the current offer is canceled in the following billing event and the new offer takes effect.

## See Also

### Promotional offers

Setting up promotional offers

Generate a key and configure offers for auto-renewable subscriptions in App Store Connect.

Generating a signature for promotional offers

Create a signature to validate a promotional offer using your private key.

Generating a Promotional Offer Signature on the Server

Generate a signature using your private key and lightweight cryptography libraries.

class SKPaymentDiscount

The signed discount to apply to a payment.

Deprecated

