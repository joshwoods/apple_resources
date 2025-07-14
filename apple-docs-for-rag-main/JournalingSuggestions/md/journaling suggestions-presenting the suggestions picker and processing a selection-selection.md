

- Journaling Suggestions
-  Presenting the suggestions picker and processing a selection 

Article

# Presenting the suggestions picker and processing a selection

Display the journaling suggestions picker and process a suggestion that someone chooses.

## Overview

Present the JournalingSuggestionsPicker to show people recent or important life events as suggestions, which include information about an event such as images, videos, locations, and so on. If a person selects a particular suggestion, the system provides you with the event details in the completion handler.

Start by choosing the text for the button in your app that presents the picker. When a person taps the text, the system presents the picker in a system process. The picker fills with suggestions that draw upon various personal experiences, such as a place someone visited, a person they connected with, a photo in their library, or a song that they often listened to.

When someone chooses a suggestion, the system makes high-level details about the event available to your app. Define the suggestion picker’s `onCompletion` closure to process the details, and incorporate them into your app’s creative workflow. A journaling app, for example, might display a visual suggestion in the format of a photo with placeholder text below it as the beginning of a new journal entry.

Journaling Suggestions gathers information from the system through built-in apps people use, such as Photos, Health, Fitness, Apple Podcasts, and Music. Suggestions can also come from third party apps that provide data through frameworks such as HealthKit, CallKit, or SiriKit.

## Maintain user privacy

Adopting Journaling Suggestions delivers an enhanced privacy experience in your app. When a person makes a selection in the picker, the system shares only the details of the chosen suggestion with your app. Thus, your app accesses only the suggestion data that a person explicitly authorizes.

When your app attempts to display the picker for the first time, a sheet appears that introduces Journaling Suggestions. If the person taps Turn On Journaling Suggestions, the picker displays, and includes an information privacy banner. The banner explains that your app only has access to the suggestions the person chooses to write about or saves to the app. The person can tap the X to close the banner, or they can tap Learn More, which presents a sheet that goes into more detail about Private Access.

- Consent sheet
- Privacy banner
- Private Access sheet

Note

The Journaling Suggestions consent sheet displays once per device, so it doesn’t appear if the person already viewed it, either by launching Journal, or by launching another app that uses Journaling Suggestions.

Suggestion data requires careful handling. To further preserve user privacy, follow the advice outlined in the Developer Program License Agreement.

## Add the Journaling Suggestions entitlement

To use Journaling Suggestions in your app, the com.apple.developer.journal.allow entitlement is required. The suggestions picker fails to present without it. You can can add this entitlement to your app by enabling the Journaling Suggestions capability in Xcode; see Adding capabilities to your app.

## Name the button that opens the suggestions picker

The JournalingSuggestionsPicker initializers take an argument, `title`, for a button that people tap to display the picker.

```
let buttonTitle = "Show my personal events"
```

Choose a title that clearly describes the purpose of journaling suggestions in the context of your app. As an indication that personal moments are about to display, it’s important to set a person’s expectations about what the picker shows after they tap the text.

## Declare and present a suggestions picker

To present a suggestions picker, declare a view that displays a button title. When a person taps the button, the system presents the picker. Upon dismissal, the system invokes the completion handler you specify.

```
struct Example: View {
    var body: some View 

## Handle the selected suggestion data

The picker fills with suggestions that include various types of personal experiences. When a person makes a selection, the system provides the chosen suggestion to your app’s `onCompletion` handler. Check the `suggestion` argument’s items property to process the selection. Each JournalingSuggestion.ItemContent item conforms to JournalingSuggestionAsset and is one of following types:

| Type | **Description** |
|----|----|
| JournalingSuggestion.Photo | An image from a person’s library, including the date captured. |
| JournalingSuggestion.Workout | Information about a workout that a person completes, including calories burnt, distance covered, a route they took, average heart rate, start and end time, and an icon for the type of workout. |
| JournalingSuggestion.Contact | An interaction a person has with someone in their contacts, including their name and Contact photo. |
| JournalingSuggestion.Location | A place that a person visited, including its name, surrounding city, and geographic coordinates, if available. |
| JournalingSuggestion.Song | The name of a song that a person plays, including the artist, album, and album artwork. |
| JournalingSuggestion.Podcast | Information about a podcast that a person plays, including the show, artist, episode, and associated artwork. |
| JournalingSuggestion.Video | A video from a person’s library, including the date captured. |
| JournalingSuggestion.LivePhoto | An image and short video that represents a live photo from a person’s library, including the date captured. |
| JournalingSuggestion.MotionActivity | The number of steps a person takes in a motion event on iPhone, including an icon for the activity. |
| JournalingSuggestion.GenericMedia | The media content a person listens to, including the information describing the media. |
| JournalingSuggestion.Reflection | A reflection prompt that a person chooses. |
| JournalingSuggestion.StateOfMind | The state of mind reflection in the Health app that describes a persons emotions and moods. |

The following example demonstrates parsing a photo suggestion:

```
struct Example: View {
    @State var suggestionPhotos = [JournalingSuggestion.Photo]()
    @State var suggestionTitle: String? = nil
    var body: some View 

The code displays the suggestion title, followed by a list of images that the person selected in the picker.

Note

A person can control the types of suggestions available in the picker by tapping Customize in the consent sheet, or by adjusting Privacy & Security settings for Journaling Suggestions in the Settings app.

When your app parses a selected suggestion’s details, it organizes that information to serve as a base for creative expression. A journaling app, for example, might list the selected images in a journal entry.

My App 1

## See Also

### Essentials

com.apple.developer.journal.allow

The entitlement that enables an app to present the journaling suggestions picker.

