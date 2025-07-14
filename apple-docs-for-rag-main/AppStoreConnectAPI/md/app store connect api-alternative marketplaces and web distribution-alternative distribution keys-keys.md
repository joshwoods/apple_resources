

- App Store Connect API
- Alternative Marketplaces and Web Distribution
-  Alternative Distribution Keys 

API Collection

# Alternative Distribution Keys

Create and manage keys for an alternative app distribution.

## Overview

As an alternative marketplace developer you create keys and JSON web tokens (JWTs) to authenticate and connect your marketplace to the apps distributed on your marketplace.

The alternative distribution key you upload to App Store Connect is a public key. Your alternative distribution key is assocaited with all alternative distribution apps in your account. You can optionally assocaite a key with a single althernative disitribution app by adding a relationship in the payload when calling Add an alternative distribution key. To learn more about creating this key, see Creating keys and establishing alternative marketplace connections.

The alternative distribution key `ID`, which you can find in the response body of the endpoint described in Read an app’s alternative distribution key is also a part of creating the JWT for Supplying an install verification token.

When using web distribution, you need to create an alternative distribution key, the private half of the key pair is used for install verification. To learn more about creating keys for web distribution, see Creating and configuring keys for web distribution. For more information, see Supplying an install verification token.

## Topics

### Creating and reading keys

Creating keys and establishing alternative marketplace connections

Manage keys you use to sign JSON web tokens and connect marketplaces with apps.

Creating and configuring keys for web distribution

Manage keys you use to sign JSON web tokens (JWTs).

Add an alternative distribution key

Add an alternative distribution key for your alternative marketplace app or web distribution.

List alternative distribution keys

List the alternative distribution key for your account.

Read alternative distribution key information

Read the public key information for a specific alternative distribution key.

Remove an alternative distribution key

Remove an alternative distribution key from your account.

### Objects

object AlternativeDistributionKey

The data structure that represents an alternative distribution key resource.

object AlternativeDistributionKeyResponse

A response that contains a single alternative distribution key resource.

object AlternativeDistributionKeysResponse

A response that contains a list of alternative distribution keys.

object AlternativeDistributionKeyCreateRequest

The request body you use to create an alternative distribution key.

## See Also

### Alternative Marketplace Setup and Configuration

Alternative Distribution Domains

Create and read alternative distribution domains.

