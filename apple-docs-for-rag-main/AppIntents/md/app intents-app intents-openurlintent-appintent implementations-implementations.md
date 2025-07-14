

- App Intents
- App intents
- OpenURLIntent
-  AppIntent Implementations 

API Collection

# AppIntent Implementations

## Topics

### Instance Properties

var systemContext: IntentSystemContext

Context information that’s available while the system performs the app intent’s action.

### Instance Methods

func callAsFunction(donate: Bool) async throws

func callAsFunction(donate: Bool) async throws -> Self.PerformResult.Value

func donate() -> IntentDonationIdentifier

Donates the intent to the transcript.

func donate() async throws -> IntentDonationIdentifier

Donates the intent to the transcript.

func donate(result: some IntentResult) -> IntentDonationIdentifier

Donates the intent and optional result to the transcript.

func donate(result: some IntentResult) async throws -> IntentDonationIdentifier

Donates the intent and optional result to the transcript.

func requestConfirmation() async throws

Requests user confirmation before performing the app intent.

func requestConfirmation(conditions: ConfirmationConditions, actionName: ConfirmationActionName, dialog: IntentDialog) async throws

Requests user confirmation before performing the app intent.

func requestConfirmation&lt;Result>(output: Result, confirmationActionName: ConfirmationActionName, showPrompt: Bool) async throwsDeprecated

func requestConfirmation&lt;Result>(result: Result, confirmationActionName: ConfirmationActionName, showPrompt: Bool) async throws

Requests user confirmation before performing the app intent.

Deprecated

### Type Aliases

typealias Case

typealias DefaultCase

typealias Parameter

typealias Summary

typealias Switch

typealias When

### Type Properties

static var authenticationPolicy: IntentAuthenticationPolicy

A property that defines the authentication policy that indicates whether this app intent requires the device to be unlocked or otherwise authenticated.

static var description: IntentDescription?

A description of the app intent that the system shows to people.

static var isDiscoverable: Bool

A boolean value that determines whether system features such as Shortcuts and Spotlight can discover this app intent.

static var openAppWhenRun: Bool

A boolean property that tells the system to consider the app intent even if its app is not in the foreground.

static var parameterSummary: some ParameterSummary

