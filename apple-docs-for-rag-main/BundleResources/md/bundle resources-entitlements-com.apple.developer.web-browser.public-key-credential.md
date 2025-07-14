

- Bundle Resources
- Entitlements
-  com.apple.developer.web-browser.public-key-credential 

Property List Key

# com.apple.developer.web-browser.public-key-credential

A Boolean value that lets your app make registration and assertion requests for passkeys and security keys for any relying party identifier.

Mac Catalyst 16.3+macOS 13.3+

## Details 

Type  

boolean

## Discussion

Only add this entitlement if your app can act as a user’s web browser.

### Web browser requirements

To request this entitlement, you must hold the Account Holder role for an organization’s Apple Developer account and complete the request form at macOS Browsers Passkeys. Apple reviews each application using predefined criteria. If your request meets the criteria, Apple adds the entitlement to your developer account using managed capabilities. For more information, see Provisioning with managed capabilities.

Apps that request this entitlement need to satisfy the following criteria:

- Your app needs to specify the HTTP and HTTPS schemes in its `Info.plist` file.

- On launch, the app needs to provide a text field for entering a URL, search tools for finding relevant links on the internet, or curated lists of bookmarks.

When opening an HTTP or HTTPS URL in its default configuration:

- The app needs to navigate directly to the specified destination and render the expected web content. Apps that redirect to unexpected locations or render content not specified in the destination’s source code don’t meet the requirements of a web browser.

- Apps that operate in a parental controls or locked down mode may restrict navigation to comply with those goals.

- Your app may present a Safe Browsing warning or other such message for suspicious content, such as phishing attempts or other concerns.

- Your app may offer a native authentication UI for a site that also offers a native web sign-in flow.

## See Also

### Web browsers

com.apple.developer.web-browser

A Boolean that indicates whether the app can act as the user’s default web browser.

com.apple.developer.browser.app-installation

The entitlement that enables a browser to install alternative-distribution apps from a website.

