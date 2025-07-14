

- Application Services
- ColorSync Manager
-  Profile Iteration Values 

# Profile Iteration Values

Specify profiles to iterate.

## Overview

These are possible values for flags passed to the function `CMIterateDeviceProfiles`.

## Topics

### Constants

var cmIterateFactoryDeviceProfiles: Int

Iterate profiles registered through the routine `CMSetDeviceFactoryProfiles`. To retrieve all factory profiles for all devices, use `cmIterateFactoryDeviceProfiles` as the flags value when calling `CMIterateDeviceProfiles`. I

var cmIterateCustomDeviceProfiles: Int

var cmIterateCurrentDeviceProfiles: Int

var cmIterateAllDeviceProfiles: Int

Iterate all profiles, without replacement.

var cmIterateDeviceProfilesMask: Int

