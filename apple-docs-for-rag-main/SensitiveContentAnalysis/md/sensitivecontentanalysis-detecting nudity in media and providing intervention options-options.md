

- SensitiveContentAnalysis
-  Detecting nudity in media and providing intervention options 

Article

# Detecting nudity in media and providing intervention options

Alert people before displaying images or video that might be sensitive.

## Overview

In iOS 17 and macOS 14, the Sensitive Content Warning user preference and Communication Safety parental control in Screen Time enable the user to indicate their desire to detect nudity in images and video. To provide people their preferred experience while those settings are active, use the SensitiveContentAnalysis framework to check incoming media before displaying it.

When the framework flags user-provided media as sensitive, intervene by adjusting the user interface in a way that explains the situation and gives the user options to proceed. Avoid displaying flagged content until the user makes a decision.

The Sensitive Content Warning setting is for adults; Communication Safety in Screen Time is intended to protect content on the devices of children. Vary your app’s intervention strategy according to the active setting. For instance, keep interaction brief and unobstructive for adults, whereas for children, use the full view and communicate in age-appropriate language.

The SensitiveContentAnalysis framework doesn’t dictate your user interface. You can tailor your app’s experience according to the examples in apps such as Messages. The following image depicts Messages in iOS 17 when a potentially explicit image arrives from a contact while the Sensitive Content Warning setting is on. Messages blurs the image with a UI that gives the user the option to display the flagged content. It also provides a menu of options to the user, such as blocking the contact or accessing Apple-provided resources on the web for topics like grooming, harassment, and online safety.

Important

Apple provides the SensitiveContentAnalysis framework to prevent people from viewing unwanted content, not as a way for an app to report on someone’s behavior. To protect user privacy, don’t transmit any information off the user’s device about whether the SensitiveContentAnalysis framework has identified an image or video as containing nudity. For more information, see the Developer Program License Agreement.

### Add the app entitlement

The OS requires the com.apple.developer.sensitivecontentanalysis.client entitlement in your app’s code signature to use SensitiveContentAnalysis. Calls to the framework fail to return positive results without it. You can can add this entitlement to your app by enabling the Sensitive Content Analysis capability in Xcode; see Adding capabilities to your app.

Any team member of the paid App Store developer program can add the entitlement to an app after enabling the capability in Xcode and then signing the Developer Program License Agreement on the Accounts website.

Note

The SensitiveContentAnalysis entitlement is not available for Enterprise development or for people with free accounts.

### Check images or video for unsafe content

To check a user-provided image for nudity, create an SCSensitivityAnalyzer object.

```
```

An app can utilize the SensitiveContentAnalysis framework by detecting sensitive content when the system sets analysisPolicy to either:

- SCSensitivityAnalysisPolicy.simpleInterventions, which indicates that the Sensitive Content Warning user preference is enabled in Settings.

- SCSensitivityAnalysisPolicy.descriptiveInterventions, which indicates that the Communication Safety settings is active in Screen Time.

An app can’t leverage the SensitiveContentAnalysis framework when the system sets analysisPolicy to SCSensitivityAnalysisPolicy.disabled. This indicates one or more of the following:

- The app lacks the necessary `com.apple.developer.sensitivecontentanalysis.client` entitlement.

- Neither the Sensitive Content Warning user preference nor the Communication Safety setting in Screen Time are active.

- One of the nudity detection settings are active, but the user disabled sensitive-content warnings for your app in Settings.

If analysisPolicy is SCSensitivityAnalysisPolicy.disabled, the SensitiveContentAnalysis framework won’t detect nudity.

```
```

If analysisPolicy is a value other than SCSensitivityAnalysisPolicy.disabled, you can check images or video for sensitive content. To check an image, call one of the `analyzeImage` functions passing in the user-provided image or a URL to an image.

```
```

To analyze a video file, pass a video URL into the `videoAnalysis` function and wait on the `hasSensitiveContent` function.

```
```

### Handle performance implications

Although sensitivity checks incur additional image processing and introduce a delay while checking video, the presence of active user preferences indicate the user’s expectation to receive protections at the cost of time to review.

Depending on the amount of time that checks take to complete, adjust your app’s UI to accommodate the delay. For example, while checking video for sensitive content, use the `progress` property on the `videoAnalysis` return value to provide the user with status in a custom UI during the process.

```
```

### Tailor user interface for the Sensitive Content Warning setting

When your app detects sensitive content, present a UI that coordinates with the active `analysisPolicy`.

When the user has enabled the Sensitive Content Warning setting, keep the user interface brief. In addition:

- Display the UI in an unobstructive manner, such as inline with other content instead of using the full screen.

- Provide intervention as the app receives sensitive content from the network but allow the app to transmit unchecked content over the network.

For example, by providing a blurred version of the potentially sensitive image in its normal location, Messages on iOS 17 and later implements *inline* intervention. Messages also keeps the information presented in the UI brief by providing a one-word button to display the image, and an icon button for more options.

### Tailor user interface for the Communication Safety parental control

When a user has enabled the Communication Safety option in Screen Time, intervene in your app as it receives sensitive content over a network, and before transmitting sensitive content over a network.

Display the intervention in a modal view and use child-appropriate language in your UI. For example, Messages on macOS 14 and iOS 17 interrupts the normal flow of the app by presenting a modal sheet that describes flagged content with broadly understood terms, such as “a naked photo”.

In addition, use two consecutive panes. The following image depicts Messages in iOS 17 when a child attempts to view a sensitive photo sent from a contact. Tapping “I’m sure” on the left raises the second pane on the right.

Inline interventions for the Sensitive Content Warning setting aim to interfere minimally with an adult’s workflow while giving them quick access to help resources. The additional navigation required in the Communication Safety setting provides children with the opportunity to make a considered choice, and tries to avoid ever catching them off guard.

