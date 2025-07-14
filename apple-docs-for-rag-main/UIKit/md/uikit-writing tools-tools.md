

- UIKit
-  Writing Tools 

API Collection

# Writing Tools

Add support for Writing Tools to your app’s text views.

## Overview

Writing Tools provides a simple way for people to improve what they write using your app. Text views that support Writing Tools gain the ability to proofread, rewrite, summarize, or compose content with the help of system-provided large language models (LLMs) and Apple Intelligence.

Writing Tools supports both the standard system views and custom text views you create. The UITextView and UITextField classes automatically support Writing Tools, but you can customize that support to suit your app’s requirements. You can also add Writing Tools support to any UIView in your app that contains text.

## Topics

### Configuration

Customizing Writing Tools behavior for UIKit views

Modify the behavior of Writing Tools in standard iOS text views, and adjust your app’s behavior while the feature is active.

enum UIWritingToolsBehavior

Constants that specify the writing tools experience for the underlying view.

struct UIWritingToolsResultOptions

Constants to specify what type of content to allow in Writing Tools suggestions or rewrites.

### Writing Tools for custom views

Adding Writing Tools support to a custom UIKit view

Add Writing Tools support, including support for inline replacement animations, to your custom iOS views that contain text.

class UIWritingToolsCoordinator

An object that manages interactions between Writing Tools and your custom text view.

protocol Delegate

An interface that you use to manage interactions between Writing Tools and your custom text view.

class Context

A data object that you use to share your custom view’s text with Writing Tools.

class AnimationParameters

An object you use to configure additional tasks or animations to run alongside the Writing Tools animations.

### Text previews

class UITargetedPreview

An object describing the view to use during preview-related animations.

class UIPreviewParameters

Additional parameters to use when animating a preview interface.

class UIPreviewTarget

An object that specifies the container view to use for animations.

## See Also

### Text

Text display and fonts

Display text, manage fonts, and check spelling.

TextKit

Manage text storage and perform custom layout of text-based content in your app’s views.

Keyboards and input

Configure the system keyboard, create your own keyboards to handle input, or detect key presses on a physical keyboard.

Handwriting recognition

Configure text fields and custom views that accept text to handle input from Apple Pencil.

