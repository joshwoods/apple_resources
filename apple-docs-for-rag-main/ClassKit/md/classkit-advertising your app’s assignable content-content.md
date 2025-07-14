

- ClassKit
-  Advertising your app’s assignable content 

# Advertising your app’s assignable content

Assemble a hierarchy of contexts and declare your app’s assignable content.

## Overview

A context, stored as a CLSContext instance, represents an area within your app, such as a book chapter or a game level, that teachers can assign to students as tasks. You create a hierarchy of contexts to enable teachers to browse and assign your app’s content. You provide deep links to the content that the contexts represent to help teachers guide students to your content. You then activate and deactivate contexts as users move through your app.

### Identify Your App’s Assignable Tasks

Before you write any new code, decide which parts of your existing app correspond to tasks that a teacher might want to assign to students. For example, a textbook reader app might divide textbooks into chapters and sections, while offering tests and quizzes to measure the reader’s retention of the material. So the app’s assignable tasks fall into a hierarchical structure with the app at the top and tests and quizzes at the bottom.

Every app that adopts ClassKit has a single, predefined top-level context called the main app context. To this, you add one or more child contexts representing assignable tasks, each potentially with descendants of its own representing subtasks.

Organize the hierarchy so that it makes sense to teachers creating assignments. For example, the lowest level contexts should represent indivisible units of work, like a quiz. Don’t define a different context for each question of a quiz when you expect teachers to assign the entire quiz as a single task. Instead, use a single context to represent the whole quiz.

Do use contexts to group other contexts in a way that allows teachers to extract useful metrics. A teacher might be interested in a student’s progress not only through a particular section of a textbook, but also through the entire chapter in which that section appears, as well as through the book as a whole. You can design a context hierarchy up to eight levels deep, including the main app context.

### Tell ClassKit About Your Content

For teachers to be able to assign your app’s content, they have to be able to see it in the Schoolwork app. Schoolwork becomes aware of your content after you tell ClassKit about it. So your next task is to declare the existence of all your contexts to ClassKit. This results in a navigable table of contents in the Schoolwork app that teachers can browse when creating assignments.

You declare a context by requesting it from the data store—the shared CLSDataStore instance—using an identifier that you assign. The act of asking for a context tells ClassKit that it exists, and where it lives in the context hierarchy. For details, see Declaring your app’s context hierarchy.

### Create New Contexts When Needed

When you ask the data store for a context, whether to declare its existence or to activate and use it, the data store looks to see if that context already exists in its database. If so, the data store returns the stored context. If not, the data store asks its delegate to build the context. You adopt the CLSDataStoreDelegate protocol to build contexts when they don’t already exist, as described in Building missing contexts.

### Help Teachers Guide Students to Your Content

Tapping in the Schoolwork app on an assignment associated with your ClassKit enabled app generates a deep link to your app. The link arrives in the form of either a user activity or a universal link, depending on how you’ve configured the context corresponding to the assignment. By properly handling this link, as described in Linking directly to assignments, you help teachers to guide students to the content that’s important to them.

### Activate Contexts When Users Begin a Task

When the user begins a task that corresponds to one of your app’s contexts, you activate the context. Later, when the user completes the task, you deactivate the context. See Informing ClassKit that a task is about to begin for details.

### Ignore the User’s Role

Certain aspects of context management only pertain to particular users. For example, students never see a complete table of contents of your app’s content in Schoolwork, so they don’t need to declare or build all contexts. They really only need to build the contexts associated with specific assignments that they receive. However, for privacy reasons, ClassKit doesn’t tell you the current user’s role. So your app must perform all operations for all users and let ClassKit figure out what data it actually needs. For more details, see About ClassKit and user roles.

## Topics

### Context management

Declaring your app’s context hierarchy

Tell ClassKit about your context hierarchy so teachers can see your assignable content.

Building missing contexts

Create and initialize missing contexts.

Informing ClassKit that a task is about to begin

Activate and deactivate contexts according to user interaction.

### Deep links

Linking directly to assignments

Make it easy for teachers to guide students to specific content.

### Bookmarks

Creating bookmarks and assignments from your app

Make it easier for teachers to find and assign your content.

## See Also

### Contexts

class CLSContext

An area of your app that represents an assignable task, like a quiz or a chapter.

protocol CLSContextProvider

An interface used to tell your ClassKit context provider app extension to update contexts.

