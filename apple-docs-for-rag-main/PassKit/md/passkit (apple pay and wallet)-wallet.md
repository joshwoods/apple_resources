

- PassKit (Apple Pay and Wallet)
-  Wallet 

API Collection

# Wallet

Manage tickets, boarding passes, payment cards and other passes in the Wallet app.

## Overview

To access your pass using PassKit add the Wallet capability to your app. You can choose to access all of the passes that are signed using your developer team identifier, or to access a subset of pass types. For information on adding capabilities to your app, see Adding capabilities to your app. For information on signing a pass, see Wallet Passes.

## Topics

### Pass library

class PKPassLibrary

Provides an interface to the user’s library of passes.

### General purpose passes

class PKSecureElementPass

A pass with a credential that the device stores in a certified payment information chip.

class PKAddSecureElementPassConfiguration

An object that describes the configuration of a secure element payment pass.

class PKAddSecureElementPassViewController

A view controller that manages the addition of secure element payment passes.

class PKPass

An object that represents a single pass.

class PKAddPassesViewController

Lets your app show a pass and prompt the user to add that pass to the pass library.

struct AsyncShareablePassConfiguration

class PKShareSecureElementPassViewController

protocol PKShareSecureElementPassViewControllerDelegate

class Preview

enum PKShareSecureElementPassResult

### Payment passes

class PKPaymentPass

An object that represents a provisioned payment card for in-app payments.

class PKAddPaymentPassViewController

Displays an interface that lets users add cards to Apple Pay from within your app.

### Stored-value passes

class PKTransitPassProperties

The properties of a transit pass.

class PKSuicaPassProperties

The properties of a pass used as a ticket for the Suica transportation system.

class PKStoredValuePassProperties

An object that represents the properties of a pass that contains a balance used for specific transactions, such as a transit pass or loyalty card.

class PKStoredValuePassBalance

An object that represents a balance that’s available for transactions, such as points or money.

### Shareable passes

class PKAddShareablePassConfiguration

An object that represents the data and action for a shared copy of pass.

class PKShareablePassMetadata

Information that you use to configure the sharing sheet for a pass.

enum PKAddShareablePassConfigurationPrimaryAction

The kind of add action that the system performs with a pass.

### Identity sheet interactions and authorization

Requesting identity data from a Wallet pass

Initiate a request for identity information by prompting a user for permission and decrypting a response payload.

Verifying Wallet identity requests

Decrypt and verify an in-app presentment request on your server.

class PKIdentityAuthorizationController

An object that presents a sheet that prompts the user to allow a request for identity information.

class PKIdentityRequest

An object that represents a request for identity information from a Wallet pass.

class PKIdentityDocument

An object that represents the response to a request.

class PKIdentityElement

An object that represents the elements an app requests from identity documents.

class PKIdentityButton

An object that displays a button to trigger the identity verification flow.

struct VerifyIdentityWithWalletButton

A view that displays a button for identity verification.

struct VerifyIdentityWithWalletButtonLabel

A type that represents the label you use with a verify identity button.

struct VerifyIdentityWithWalletButtonStyle

A type that represents the style you use with a verify identity button.

### Digital car keys

class PKAddCarKeyPassConfiguration

A specialized configuration object that PassKit uses when it creates a digital car key.

class PKVehicleConnectionSession

protocol PKVehicleConnectionDelegate

enum PKVehicleConnectionSessionConnectionState

### Extend Wallet to add issuer cards

Implementing Wallet Extensions

Support adding an issued card to Apple Pay from directly within Apple Wallet using Wallet Extensions.

class PKIssuerProvisioningExtensionHandler

An abstract superclass for an app extension to add a payment card to Wallet.

protocol PKIssuerProvisioningExtensionAuthorizationProviding

A protocol for a UI app extension to authorize a user to add a payment card to Wallet.

### Common objects

Common data types that are used throughout the Wallet.

class PKObject

An opaque type that acts as the superclass for the pass object.

class PKAddPassButton

Provides a button that enables users to add passes to Wallet.

class PKLabeledValue

An object that can represent a detail about a payment card or other item.

struct AddPassToWalletButton

struct AddPassToWalletButtonFilter

struct AddPassToWalletButtonResponse

struct AddPassToWalletButtonStyle

### Entitlements

Pass Type IDs Entitlement

A list of identifiers that specify pass types that your app can access in Wallet.

### Errors

struct PKPassKitError

Errors that the PassKit framework uses.

struct PKAddSecureElementPassError

An error object that PassKit uses when it adds Secure Element passes.

enum Code

Errors that the PassKit framework uses.

enum Code

Error codes for problems that occur when you add a secure element passes.

enum PKAddPaymentPassError

Error codes for adding payment passes.

struct PKIdentityError

A structure that represents an identity error.

enum Code

Error codes for identity operations.

struct PKShareSecureElementPassError

enum Code

enum PKVehicleConnectionErrorCode

enum PayWithApplePayButtonPaymentAuthorizationPhase

let PKPassKitErrorDomain: String

The error domain for PassKit errors.

let PKIdentityErrorDomain: String

The error domain for identity errors.

let PKAddSecureElementPassErrorDomain: String

The error domain for errors that occur when adding a secure pass.

let PKShareSecureElementPassErrorDomain: String

### Japan passes

struct JPKIPassContents

A set of actions for viewing and updating PINs, passwords, and signing abilities associated with digital identities on the JPKI applet.

class PKAddIdentityDocumentConfiguration

Configuration to define the identity document.

class PKAddPassMetadataPreview

A preview object that contains information representing the pass you add to Wallet.

class PKIdentityDocumentMetadata

A set of configured metadata defining the required information to add the corresponding pass to Wallet.

class PKIdentityNationalIDCardDescriptor

An object for requesting information from a user’s national ID card.

class PKJapanIndividualNumberCardMetadata

A class that contains metadata indicating the specific product instance to provision.

### Deprecated

struct PayLaterView

A view that displays the Apple Pay Later visual merchandising widget.

Deprecated

class PKPayLaterView

A view that displays the Apple Pay Later visual merchandising widget.

Deprecated

## See Also

### Related Documentation

Wallet Passes

Create, distribute, and update passes for the Wallet app.

