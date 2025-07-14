

- Authentication Services
-  Simplifying User Authentication in a tvOS App 

Sample Code

# Simplifying User Authentication in a tvOS App

Build a fluid sign-in experience for your tvOS apps using AuthenticationServices.

Download

tvOS 15.0+Xcode 13.0+

## Overview

Note

This sample code project is associated with WWDC21 session 10279: Simplify sign in for your tvOS apps.

### Configure the Sample Code Project

To configure the sample code project, perform the following steps in Xcode:

1.  Add your Apple ID account and assign the target to a team so Xcode can enable the `Associated Domains` capability with your provisioning profile.

2.  Configure your web credentials domain in the `Associated Domains` capability and your website’s associated domains file.

3.  Set up an Apple TV running tvOS 15 and an iPhone or iPad running iOS 15 or iPadOS 15.

4.  Add the same Apple ID to both devices. Alternatively, you may pair the iPhone or iPad with the Apple TV.

5.  Set the Apple TV as the run destination in the scheme pop-up menu.

6.  In the toolbar, click Run, or choose Product \> Run.

## See Also

### Sign In with Apple

Implementing User Authentication with Sign in with Apple

Provide a way for users of your app to set up an account and start using your services.

struct SignInWithAppleButton

The view that creates the Sign in with Apple button for display.

Sign in with Apple Entitlement

An entitlement that lets your app use Sign in with Apple.

class ASAuthorizationAppleIDProvider

A mechanism for generating requests to authenticate users based on their Apple ID.

class ASAuthorizationAppleIDCredential

A credential that results from a successful Apple ID authentication.

