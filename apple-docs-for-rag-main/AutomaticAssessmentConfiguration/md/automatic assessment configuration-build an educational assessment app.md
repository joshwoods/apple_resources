

- Automatic Assessment Configuration
-  Build an Educational Assessment App 

Sample Code

# Build an Educational Assessment App

Ensure the academic integrity of your assessment app by using Automatic Assessment Configuration.

Download

macOS 12.0+Xcode 13.3+

## Overview

Academic assessment apps need to ensure that students can’t use certain system resources, like network access, the dictionary, and the calculator. However, depending on the assessment, you might want to allow students to use one or more of these resources. Use the Automatic Assessment Configuration framework to enable assessment administrators to chose which of these system resources, if any, students can use during an assessment.

This app is a web browser, with a Lock and Unlock button to enter and exit from Assessment mode, and additional buttons that can configure and launch the participating Calculator and Dictionary apps with varying participant app configurations. These configurations are:

- No access, where the participant app is prevented from launching

- Allowed, with no network access, where the participant app can launch, but it can’t access the network

- Allowed, with full network access, where the participant app can launch, and it has full network access

You can choose either Objective-C or Swift to build and run the same sample app.

### Configure the Sample Code Project

To build and run this sample on your device, you must first select your development team for the project’s target using these steps:

1.  Change the sample project’s bundle ID to something unique.

2.  Make sure your team has been granted the com.apple.developer.automatic-assessment-configuration entitlement for macOS.

3.  Create an App ID with this capability on the Provisioning Portal. Make sure the ID matches the bundle ID.

4.  Create a Provisioning Profile for Mac Development with the App ID you created.

5.  For the project’s target, choose your team from the Team menu in the Signing & Capabilities pane, and deselect the checkbox so Xcode won’t automatically manage code signing.

6.  In the Provisioning Profiles drop-down, chose to download profiles.

### Start the Assessment Session

Before the app can start an assessment session, it needs to initialize the session.

```
// Start with an assessment configuration.
AEAssessmentConfiguration *config = [[AEAssessmentConfiguration alloc] init];
```

Then the app configures one or more apps that the student is allowed to use during the assessment. The sample creates AEAssessmentParticipantConfiguration instances to allow or disallow network access.

```
// A configuration that allows network access.
AEAssessmentParticipantConfiguration *networkAllowedConfig = [[AEAssessmentParticipantConfiguration alloc] init];
networkAllowedConfig.allowsNetworkAccess = true;

// A configuration that prevents network access.
AEAssessmentParticipantConfiguration *noNetworkConfig = [[AEAssessmentParticipantConfiguration alloc] init];
noNetworkConfig.allowsNetworkAccess = false;
```

The sample then configures an app with one of the previously created `AEAssessmentParticipantConfiguration` instances, as appropriate, by calling an AEAssessmentConfiguration instance’s setConfiguration(_:for:) method.

```
AEAssessmentApplication *calculator = [[AEAssessmentApplication alloc] initWithBundleIdentifier:calculatorBundleID];

switch ( [self.calculatorOptions selectedSegment] ) {
    case 0: // Not allowed.
        [self log:@"Calculator will not be allowed when locked"];
        break;
    case 1: // Allowed, no network.
        [self log:@"Calculator will be allowed when locked, with no network access."];
        [config setConfiguration:noNetworkConfig forApplication:calculator];
        break;
    case 2:  // Allowed, with network.
        [self log:@"Calculator will be allowed when locked, with network access."];
        [config setConfiguration:networkAllowedConfig forApplication:calculator];
        break;
    default:
        [self log:@"Unexpected segment; Calculator not allowed."];
        break;
}
```

Finally, the sample starts the assessment session.

```
[self.session begin];
```

### Handle Assessment Session Events

Implement the AEAssessmentSessionDelegate methods to be notified of assessment session lifecycle events. For example, the assessmentSession(_:wasInterruptedWithError:) delegate method handles the case of a system failure interrupting the assessment session.

```
- (void)assessmentSession:(AEAssessmentSession *)session wasInterruptedWithError:(NSError *)error {
    [self log:@"Session interrupted - %@", [error localizedDescription]];
    [session end];
    [self updateLockButton];
}
```

### End the Session

When the student finishes taking the assessment, save the results and end the assessment session.

```
[self.session end];
```

## See Also

### Sessions

Preparing an educational assessment app for distribution

Ensure your app maintains academic integrity by reviewing assessment practices and managing system capabilities.

class AEAssessmentConfiguration

Configuration information for an assessment session.

class AEAssessmentSession

A session that your app uses to protect an assessment.

