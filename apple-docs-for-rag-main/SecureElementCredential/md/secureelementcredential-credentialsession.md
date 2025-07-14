

- SecureElementCredential
-  CredentialSession 

Class

# CredentialSession

A class for performing actions on a credential stored in the Secure Element.

iOS 18.1+iPadOS 18.1+

``` source
actor CredentialSession
```

## Mentioned in 

Accessing and using secure element credentials

## Overview

Create a credential session with the startSession() method. After you start a session, the session has three states:

Management  
In this default state, you can list, add, and delete credentials in the Secure Element.

Wired  
The wired state allows you to exchange data with a credential-corresponding entity (an *applet*) in the Secure Element.

Card Emulation  
In the card emulation state, your credential can communicate with a contactless card reader.

The framework provides SwiftUI and UIKit user interfaces for your app to display while using the wired and card emulation states.

You can read the current state at any time from the state property. The eventStream property provides an AsyncStream of events from both your own actions on credentials and outside sources like detecting an NFC reader’s RF field.

An app can have only one active session at a time. When your app no longer needs the credential session, call invalidate(). If your app goes into the background, the system automatically invalidates your session after a short delay. In wired mode, the system invalidates the session if it goes 15 seconds without performing a transceive(_:) call.

## Topics

### Verifying eligibility

static var isEligible: Bool

Clients should always check if this variable returns true to dynamically determine if the current device and user configuration can utilize this service before starting a session with this client

### Accessing hardware information

var secureElementInfo: CredentialSession.SecureElementInfo

A property that provides information about the Secure Element hardware.

struct SecureElementInfo

A type that provides information about the Secure Element hardware.

### Managing the credential session life cycle

static func startSession() async throws -> CredentialSession

Requests a session to view, manage, or use credentials in the Secure Element.

func invalidate() async throws

Inmediately invalidates a session.

### Accessing the session state

var state: CredentialSession.State

The current state of the session.

enum State

An enumeration of the possible states of a card session.

### Accessing credentials

func listCredentials() async throws -> [CredentialSession.Credential]

Retrieves a list of of credentials to which the app has access rights.

struct Credential

Information about a credential that a credential session retrieves from the Secure Element.

### Acquiring exclusive foreground privileges

func acquirePresentmentAssertion() async throws -> CredentialSession.PresentmentIntentAssertion

Indicates that the app intends to present a credential to a contactless interface.

class PresentmentIntentAssertion

An object that signals your app’s intention to make exclusive use of the device’s contactless features.

### Handling session events

var eventStream: AsyncStream&lt;CredentialSession.Event>

An asynchronous stream of session events.

enum Event

Events produced by a credential session, such as connectivity events and errors.

### Managing a credential

func provisionCredential(configurationUUID: UUID, name: String) async throws -> CredentialSession.Credential

Creates a credential in the Secure Element.

func deleteCredential(CredentialSession.Credential) async throws

Deletes a credential on the Secure Element.

### Performing wired mode actions

func performWiredTransaction(using: CredentialSession.Credential, over: UIScene, instanceAID: Data) async throws

Enters wired mode with user authentication.

func enterWiredMode(using: CredentialSession.Credential) async throws

Enters wired mode to perform maintenance operations with the given credential.

func transceive(Data) async throws -> Data

Send a wired command Application Protocol Data Unit (APDU) to the credential.

func endWiredMode() async throws

Ends wired mode and returns to management state.

### Performing card emulation

func performCardEmulationTransactionWithCurrentCredential(over: UIScene, options: CredentialSession.CardEmulationOptions) async throws

Activate the current credential in Wired mode to enter Card Emulation mode.

func performTransaction(using: CredentialSession.Credential, over: UIScene, options: CredentialSession.CardEmulationOptions) async throws

Prompts the user for authorization and then activate a credential for card emulation.

struct CardEmulationOptions

Options for customizing card emulation behavior.

func endCardEmulation() async throws

Ends card emulation and transitions the session to management state.

### Using SwiftUI

func configuration() async throws -> CredentialTransaction.Configuration

Retrieves a transaction configuration related to this session.

class Configuration

An object that provides configuration information for a transaction that the client intends to peform.

### Handling errors

enum ErrorCode

An error encountered by a credential session.

### Working with actors

var unownedExecutor: UnownedSerialExecutor

Retrieve the executor for this actor as an optimized, unowned reference.

### Comparing sessions

static func == (CredentialSession, CredentialSession) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Infrequently-used functionality

init()

Creates an empty credential session.

### Structures

struct ConnectivityEvent

An event that a credential receives during card emulation.

### Enumerations

enum NFCFieldInformation

The state of an NFC RF field.

### Default Implementations

Actor Implementations

Equatable Implementations

## Relationships

### Conforms To

- Actor
- Equatable
- Sendable

