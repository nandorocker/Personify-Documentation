### Personify Collaboration v 1.0.0

# Design Guidelines

By [nando rossi](mailto:talk@nan.do)



### Introduction

This guide is intended as a way to assist implementation of the Personify Application designs. The document is being initially created with the Windows version in mind; as we roll out other platforms, the details specific to them will be included, although we will keep a goal in mind: a **unified vision**.

### The Vision

The goal of this app is to promote collaboration and bring people closer together using technology in a seamless way.

- All Personify apps should **Feel** like Personify. They must "speak" to one another visually, regardless of platform
- Interface should always be as minimal as possible. The **work** and the **people** should be at the front and center.
- Take advantage of the platform. Before implementing Personify to a new platform, consider that platform's strengths and weaknesses, and look at each feature individually:
	- What types of input work best in this platform?
	- Can this feature be "translated" in a way that is logically similar to the other platforms, and yet follows this platform's best practices?
	- Does this feature **make sense** in this platform? Is it essential?
- Build from the ground up. Get the simple things **right** first, then complicate it. It's much easier to see what works and what doesn't when you start small than when you have to trim it down.

### Global Styles

## Fonts & Palette

### Segoe UI

The main font used for Personify is **Segoe UI**, which is also the font most commonly associated with the Windows "Modern" interface. It's clear, it's international and although it's a Windows font, it can exist well outside of it.

It is also a modern sans-serif font, but not the over-used (and at the moment very associated with Apple) Helvetica.

These weights will be used throughout the app:

- Light
- Semilight
- Normal
- Semibold

Font sizes try to follow the **Modular Scale** whenever possible (there are some exceptions):
9, 10, 11, 12, 13, 14, 18, 20, 24, 36, 48, 64, 72, 144, 288


### Colors

The entire palette for the app stems from these main colors:

- White: `#FFFFFF`
- Light Blue: `#00B0FF`
- Dark Blue: `#3E484C`
- Red: `#D05F5`

## Iconography

- Friendly but adult
- Single-color icons (some icons can also feature a 40% opacity version of the color)
- Universally recognizable icons should be used whenever possible (such as **share** and **x** for closing)
- The **phone** metaphor is used when referencing 

## Window design
- As minimal as possible, to let users see work/shared windows/each other as much as possible
- Self-contained; focus the action on the Toolbar window
- Use modals whenever possible instead of "sticky" windows
- Allow user to make windows "stick"


### App sections

## Onboarding

## Home & Login

### The Login screen

#### Styles
![image](images/Login.png)

![image](images/Login - Error.png)

### Home Screen

#### Styles

![image](images/Home Window.png)

### Starting a call

#### Styles
![image](images/Home Window - Start Call.png)
Start a call

![image](images/Home Window - Recent calls.png)
Recent Calls

![image](images/Add a User - 02 - Recent.png)
New Call - Recent callers

![image](images/Add a User - 03 - Suggest.png)
New Call - Autosuggest

![image](images/Add a User - 03 - Suggest 2.png)
New Call - Copy Link

## In-call

### App parts


### The Toolbar


### The Thumbnail Bar



## Manipulating Personas

## Chat

## Screen Sharing

## Screen Recording