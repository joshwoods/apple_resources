

- Apple Pay on the Web
-  Choosing an API for Implementing Apple Pay on Your Website 

Article

# Choosing an API for Implementing Apple Pay on Your Website

Compare Apple Pay JS and Payment Request API to choose the right implementation for your website.

## Overview

Safari supports two APIs for implementing payment requests: Apple Pay JS API, and the W3C Payment Request API. Both APIs present the same Apple Pay payment sheet on Safari, and offer nearly the same user experience.

To help you decide which API to implement, or whether to implement both, first determine which features your solution requires, and choose the API that matches your needs.

### Features of Apple Pay JS API

Use Apple Pay JS API if you depend on any of its unique features:

**Granular error handling.** You can provide robust error handling:

- Customizable error messages and field indications create a better user experience. See ApplePayError for more information.

- You can report errors the user can correct, even after the user authorizes payment.

- You can retry if an error occurs after the user authorizes payment. With Payment Request API, the user must restart their transaction.

**Integration for store cards and cobranded debit/credit cards.** When customers with affiliated cards visit your website, you can provide these additional benefits:

- Apple Pay can automatically select the affiliated card instead of the customer’s default card.

- You can adjust prices or other terms of a sale for customers using your affiliated card. For example, you might provide free shipping when customers use your cobranded VISA credit card.

**Phonetic names.** You can request a phonetic name in Apple Pay JS API only.

### Features of Payment Request API

Use Payment Request API for these benefits:

- **Cross-browser solution.** Payment Request API-based code can support a variety platforms and browsers. Apple Pay is available on Safari; other payment methods are available on other browsers and platforms.

- **W3C standard candidate API.** The Payment Request API is defined by the World Wide Web Consortium (W3C).

### Choose an API to Support Your Customers

To better reach your customers, choose an API that works on their devices, as follows:

- **Apple Pay JS API:** Supported in iOS 10 and later, and macOS 10.12 and later.

- **Payment Request API:** Supported in iOS 11.3 and later, and Safari 11.1 on macOS 10.12 and later.

When implementing Payment Request API, consider also implementing Apple Pay JS API as a fallback for customers whose devices run an older operating system version.

### Requirements for Both APIs

The same first steps, configurations, and guidelines for using Apple Pay on the web apply regardless of which API you choose to implement.

For more information, see Apple Pay setup, Apple Pay buttons, and for design guidance see Human Interface Guidelines > Apple Pay on the Web.

## See Also

### Apple Pay JavaScript APIs

Apple Pay on the Web version history

Learn about features in each version of Apple Pay on the Web.

Apple Pay JS API

Implement Apple Pay on the web using Apple’s JavaScript API.

Payment Request API

Accept payments on your website with Apple Pay using the Payment Request API.

