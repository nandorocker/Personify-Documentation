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
(add this)

## Home & Login

### Login screen

#### Login

![image](images/Login.png)

##### Login - Error

![image](images/Login - Error.png)

### Home Screen

#### Home Screen

![image](images/Home Window.png)

### Starting a call

#### Start a call

![image](images/Home Window - Start Call.png)

#### Recent calls

![image](images/Home Window - Recent calls.png)

#### New Call - Recent callers

![image](images/Add a User - 02 - Recent.png)

<a name="autosuggest"></a>
#### New Call - Autosuggest

![image](images/Add a User - 03 - Suggest.png)

#### New Call - Copy Link

![image](images/Add a User - 03 - Suggest 2.png)

#### Receiving a call

![image](images/Receiving a call.png)


## In-call

### The Toolbar

#### Single user

![image](images/Toolbar - Single user in call.png)


### The Thumbnail Bar

(add this)

### Add user in-call

![image](images/Add User - 01 - Type name.png)

Step 1 - modal overlay on thumbnail screen  
Step 2 - as user types, see [autosuggest](#autosuggest).

## Manipulating Personas

### The "Interaction Radius"

![image](images/Manipulating - 01 - Interaction Radius.png)

(describe & explain this)

### Moving personas left-right

As a user, I want to move my *persona* around to allow me to see my work/other windows.

As I move my cursor towards the *persona*, it fades out, but a blue box is still visible. I can click on that box and drag the persona side-to-side, and it's anchored to the bottom of the screen.

![image](images/Manipulating - 02 - Cursor Within Radius.png)

![image](images/Manipulating - 03 - Moving Persona 1.png)

![image](images/Manipulating - 04 - Moving Persona 2.png)

![image](images/Manipulating - 05 - Moving Persona 3.png)

(design this)

If I move the box **upwards**, the box displays an "up arrow" and if I let go, the persona moves up to the "thumbnail box" (with a nice transition animation).

## Chat

#### Chat Window & Speech bubbles

As a user, I want to send messages and files to my chat partners without disrupting my workflow.

I can click on the "messages" icon.
A **modal** is displayed, with:

- Text field
- "Upload file" button
- "Conversation" button

I can type a message on the text field, and it gets sent to all users as a "chat bubble", which gets displayed and goes away. Uploaded files have the same effect.
![image](images/Chat - 01.png)

I can click the "conversation" button and it fires up a standard "chat" window, which should then disable the "chat bubbles" (only for as long as it's focused).

![image](images/Chat - 02.png)

## Screen Sharing

As a user, I want to share an application I'm using with my chat partners.

I can click the **screen share button**

![image](images/Share - 01 start.png)

Which displays a "select window" dialog. I can then select which window to share.

![image](images/Share - 02 - select window.png)

The window I'm currently sharing will take on a thick outline to make it clear.

![image](images/Share - 03 - sharing active.png)

## Screen Recording

As a user, I want to create and share videos of my screen while I perform a variety of activities.

- At the home screen, I roll over the "Screen Recording" button
- I then select "new recording"

![image](images/Home Window - Screen Recording.png)

![image](images/Recording setup raw.png)

![image](images/Recording setup.png)

Recording - Styles

I choose my settings and then click "start recording."

![image](images/Countdown.png)

There is a countdown, I record. 

![image](images/Recording.png)

When I'm done, I press the "stop" button and the video gets uploaded.

![image](images/Uploading.png)

![image](images/Upload successful.png)

While the file uploads, I can share the video, or copy the link to it.

![image](images/Sharing Video.png)