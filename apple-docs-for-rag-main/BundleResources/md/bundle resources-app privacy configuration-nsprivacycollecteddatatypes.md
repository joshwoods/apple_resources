

- Bundle Resources
- App Privacy Configuration
-  NSPrivacyCollectedDataTypes 

Property List Key

# NSPrivacyCollectedDataTypes

A list of dictionaries that report the categories of private data your app or third-party SDK collects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 14.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

## Details 

Name  
Privacy Nutrition Label Types

Type  

array of dictionaries

## Mentioned in 

Describing data use in privacy manifests

## Overview

For more information, see Describing data use in privacy manifests.

## Topics

### Reporting categories of collected data

NSPrivacyCollectedDataType

A string that identifies the type of data your app or third-party SDK collects.

**Name:** Collected Data Type

NSPrivacyCollectedDataTypePurposes

An array of strings that identify reasons your app or third-party SDK collects private data.

**Name:** Collection Purposes

### Reporting tracking and linking collected data

NSPrivacyCollectedDataTypeLinked

A Boolean that indicates whether your app or third-party SDK links this data type to the user’s identity.

**Name:** Linked to User

NSPrivacyCollectedDataTypeTracking

A Boolean that indicates whether your app or third-party SDK uses this data type to track.

**Name:** Used for Tracking

