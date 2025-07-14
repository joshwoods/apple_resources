

- StoreKit Test
-  SKAdTestPostbackVersion 

Structure

# SKAdTestPostbackVersion

A constant that indicates the postback version.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
struct SKAdTestPostbackVersion
```

## Overview

This postback version number corresponds to a version of SKAdNetwork. All versions of SKAdNetwork have specific instructions for signing ads and validating postbacks. The testing environment supports testing the versions indicated by the constants listed in the Getting SKAdNetwork Versions section below.

For more information about versions, see SKAdNetwork release notes.

## Topics

### Getting SKAdNetwork Versions

static let version4_0: SKAdTestPostbackVersion

A constant that represents SKAdNetwork version 4.0.

static let version3_0: SKAdTestPostbackVersion

A constant that represents SKAdNetwork version 3.0.

static let version2_2: SKAdTestPostbackVersion

A constant that represents SKAdNetwork version 2.2.

static let version2_1: SKAdTestPostbackVersion

A constant that represents SKAdNetwork version 2.1.

### Initializing the Postback Version

init(rawValue: String)

Initialize a version object with the supplied raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Ad impression and postback testing

Testing and validating ad impression signatures and postbacks for SKAdNetwork

Validate your ad impressions and test your postbacks by creating unit tests using the StoreKit Test framework.

class SKAdTestSession

The class you use to test ad impressions and postbacks in Xcode.

class SKAdTestPostback

A test postback that contains ad conversion information in the testing environment.

class SKAdTestPostbackResponse

The status and error information for a postback that the system sends in the testing environment.

