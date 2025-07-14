

- Bundle Resources
-  App Privacy Configuration 

Property List

# App Privacy Configuration

A data structure that represents the root object in a privacy manifest file.

iOS 17.0+iPadOS 17.0+Mac Catalyst 14.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

## Details 

Type  

object

## Overview

Use the keys and values in this object in the privacy manifest for your app or third-party SDK. For more information, see Privacy manifest files.

## Topics

### Describing privacy accessed API use

NSPrivacyAccessedAPITypes

A list of dictionaries that report the privacy accessed API your app or third-party SDK uses.

**Name:** Privacy Accessed API Types

### Describing collected data

NSPrivacyCollectedDataTypes

A list of dictionaries that report the categories of private data your app or third-party SDK collects.

**Name:** Privacy Nutrition Label Types

### Declaring tracking

NSPrivacyTracking

A Boolean value that indicates whether your app or third-party SDK uses data for tracking.

**Name:** Privacy Tracking Enabled

NSPrivacyTrackingDomains

A list of the internet domains your app or third-party SDK uses for tracking.

**Name:** Privacy Tracking Domains

## See Also

### Essentials

Adding a privacy manifest to your app or third-party SDK

Report the data you collect and the required reasons API you use in your app or third-party SDK.

Describing data use in privacy manifests

Declare the data collected by your app or by third-party SDKs.

Describing use of required reason API

Ensure your use of covered API is consistent with policy.

