

- App Store Connect API
- App Store
- App Clips and App Clip Experiences
-  Default App Clip Experiences 

API Collection

# Default App Clip Experiences

Read, create, update, and delete your default App Clip experience.

## Overview

The `appClipDefaultExperiences` resource provides functionality to read information about the default App Clip experience you configure for your App Clip. Additionally, it provides functionality to create a default App Clip experience, to update an existing default App Clip experience, and to delete an unreleased default App Clip experience.

## Topics

### Getting Default App Clip Experience Information

Read Default App Clip Experience Information

Get a specific default App Clip experience.

Read the App Store Review Detail for a Default App Clip Experience

Get App Store Review details for a specific default App Clip experience.

Read Localization Information for a Default App Clip Experience

Get localized metadata that appears on the App Clip card for a specific default App Clip experience.

Read App Store Version Information for a Default App Clip Experience

Get App Store Version information for a default App Clip experience.

Get the App Store Versions Resource ID for a Default App Clip Experience

Get IDs for App Store Versions related to a default App Clip experience.

### Managing Default App Clip Experiences

Create a Default App Clip Experience

Configure a new default App Clip experience.

Modify a Default App Clip Experience

Update a default App Clip experience.

Modify the Related App Store Version for a Default App Clip Experience

Update the relationship between a default App Clip experience and an App Store Version.

Delete a Default App Clip Experience

Delete a specific default App Clip experience.

### Managing Default App Clip Experience Metadata

App Clip Header Images

Read and manage image assets that appear on the App Clip card.

Default App Clip Experience Localizations

Read and manage the metadata of your default App Clip experience.

### Objects and Types

object AppClipDefaultExperience

The data structure that represents a Default App Clip Experiences resource.

object AppClipDefaultExperienceResponse

A response that contains a single Default App Clip Experiences resource.

object AppClipDefaultExperienceCreateRequest

The request body you use to create a default App Clip experience.

object AppClipDefaultExperienceUpdateRequest

The request body you use to update a default App Clip experience.

object AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest

The request body you use to relate a released App Store version with a default App Clip experience.

object AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse

A response that contains the ID of a single related App Store Versions resource.

type AppClipAction

A string that represents the call- termto- termaction verb on the App Clip card.

## See Also

### Managing App Clip Experiences

Advanced App Clip Experiences

Create, read, update, and delete your advanced App Clip experiences.

