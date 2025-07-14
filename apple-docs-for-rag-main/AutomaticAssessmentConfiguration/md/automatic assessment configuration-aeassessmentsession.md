

- Automatic Assessment Configuration
-  AEAssessmentSession 

Class

# AEAssessmentSession

A session that your app uses to protect an assessment.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
class AEAssessmentSession
```

## Overview

Use the AEAssessmentSession class to manage an assessment session. The system allows only one active session at a time across all processes. The first session to run gets exclusive access to the system; subsequent session attempts fail until the first session ends.

To create an assessment session, pass a new AEAssessmentConfiguration instance to the init(configuration:) method. Then, provide the session with a delegate that conforms to the AEAssessmentSessionDelegate protocol:

- Swift
- Objective-C

```
let config = AEAssessmentConfiguration()
let session = AEAssessmentSession(configuration: config)
session.delegate = self
```

```
AEAssessmentConfiguration *config = [AEAssessmentConfiguration new];
AEAssessmentSession *session = [[AEAssessmentSession alloc] initWithConfiguration:config];
session.delegate = self;
```

You can indicate exceptions to the restrictions imposed by an assessment session by setting the properties of the configuration instance, or you can use the default restrictions as shown above. The session tells its delegate about state changes during its life cycle. To start a session, call the session’s begin() method:

- Swift
- Objective-C

```
session.begin()
```

```
[session begin];
```

The method returns immediately, and the session starts disabling system features. After achieving the desired state, the session calls its delegate’s assessmentSessionDidBegin(_:) method. Only after receiving this callback is it safe to begin your assessment. Be sure to keep a strong reference to the session as long as you want it to remain active. If the system deallocates an active session, the session automatically ends.

Important

Prior to macOS 12.1, a DNS lookup that your app initiates during a session might fail. Be sure your app resolves all required domain names before beginning a session so that the system can cache the results. You can do this by using URLSession to send a `HEAD` request to each domain name that your app needs to access.

After completing an assessment and hiding all sensitive information, call the session’s end() method:

- Swift
- Objective-C

```
session.end()
```

```
[session end];
```

After making the call, wait for the session to call its delegate’s assessmentSessionDidEnd(_:) method before reporting assessment completion to the user.

During assessment, the session’s delegate might receive an assessmentSession(_:wasInterruptedWithError:) callback to indicate a failure. If this happens, immediately stop the assessment, hide all sensitive content, and end the session. Because it might take time for your app to finalize the assessment, the session relies on your app to call the session’s end() method:

- Swift
- Objective-C

```
func assessmentSession(_ session: AEAssessmentSession, wasInterruptedWithError error: Error) {
    // Hide sensitive UI and optionally store assessment progress.

    // End the session.
    session.end()
}
```

```
- (void)assessmentSession:(AEAssessmentSession *)session wasInterruptedWithError:(NSError *)error {
    // Hide sensitive UI and optionally store assessment progress.

    // End the session.
    [session end];
}
```

## Topics

### Creating a session

init(configuration: AEAssessmentConfiguration)

Creates a new assessment session.

### Managing session configuration

func update(to: AEAssessmentConfiguration)

Changes the session to use the specified configuration.

var configuration: AEAssessmentConfiguration

The current configuration of the session.

class var supportsMultipleParticipants: Bool

A Boolean that indicates whether the current device or platform supports a configuration with one or more participant applications.

class var supportsConfigurationUpdates: Bool

A Boolean that indicates whether the current device or platform supports updating a session’s configuration after the session has begun.

### Responding to session updates

var delegate: (any AEAssessmentSessionDelegate)?

A delegate to which the session provides state change updates.

protocol AEAssessmentSessionDelegate

An interface that the session uses to provide information about session state changes to a delegate.

### Starting and stopping a session

func begin()

Starts an assessment session.

func end()

Ends an assessment session.

var isActive: Bool

A Boolean that indicates whether an assessment session is running.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Sessions

Preparing an educational assessment app for distribution

Ensure your app maintains academic integrity by reviewing assessment practices and managing system capabilities.

Build an Educational Assessment App

Ensure the academic integrity of your assessment app by using Automatic Assessment Configuration.

class AEAssessmentConfiguration

Configuration information for an assessment session.

