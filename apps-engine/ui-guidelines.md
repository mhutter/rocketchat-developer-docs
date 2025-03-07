# UI Guidelines

Follow these guidelines for any interface you are creating for your Rocket.Chat App using the Apps Engine.

## Surface Types

There are two surfaces types:

1. **Simple**: Simple surface types are examples like menus that can contain only the predefined list of menu items
2. **Complex**: Examples like contextual bars and modals which can use all available [UiKit ](fundamentals-of-apps/uikit/)components to build the intended user experience.

## User Menu

The user menu contains items specific to the user such as status and preferences. Every item on this menu should relate to a user.

* Add only user-specific items to this menu

<figure><img src="../.gitbook/assets/User menu visual guide.png" alt=""><figcaption><p>User menu visual guide</p></figcaption></figure>

## Room kebab menu

The room kebab menu is located at the top right of any [Rocket.Chat Room](https://docs.rocket.chat/use-rocket.chat/user-guides/rooms).

* This menu opens up a contextual bar and not a modal.
* Items on this menu must relate to or affect the current room or its context in some way.
* Do not include icons or use emojis in item labels.

<figure><img src="../.gitbook/assets/Room kebab menu UI guide.png" alt=""><figcaption><p>Room kebab menu UI guide</p></figcaption></figure>

## Message kebab menu

The message kebab menu can be seen by the right of a message when hovered upon on a Desktop or long-pressed on a Mobile device.

* The message kebab menu is reserved exclusively for items that affect the selected message.
* Only Rocket.Chat core actions can use icons.
* Do not include icons or emoji anywhere inside the item label.

<figure><img src="../.gitbook/assets/Message kebab menu UI guide.png" alt=""><figcaption><p>Message kebab menu UI guide</p></figcaption></figure>

## Chat messages

* Make messages very clear, brief, and not long.
* Do use an emoji if only they help get the intended message across.
* Do not send messages on a user's behalf.
* Do not over-communicate or use emojis excessively.

<figure><img src="../.gitbook/assets/Chat message UI Guide.png" alt=""><figcaption><p>Chat message UI Guide</p></figcaption></figure>

## Slash commands

Slash commands are usually the simplest ways users can interact with installed apps.

* Slash command descriptions should appear by the side of the command when typed in the message composer.
* Commands must have hyphens between words and include a description.

<figure><img src="../.gitbook/assets/Slash commands UI Guide.png" alt=""><figcaption><p>Slash commands UI Guide</p></figcaption></figure>

* All apps using a slash command must have a `/help` command showing the possibilities of the app and it's commands

## Contextual bars

Apps can utilize the contextual bar surface to offer information and actions to the user.

* Contextual bars must contain a corresponding item in the [room kebab menu](ui-guidelines.md#room-kebab-menu).
* Contextual bar titles must use sentence case capitalization eg: `Google Calendar settings` not `Google Calendar Settings.`
* Do not use images, such as app icons, inside the contextual bar header.
* Do not use titled case in the contextual bar header.
* Do use sentence case in contextual bar header.

<figure><img src="../.gitbook/assets/Contextual bar UI Guide.png" alt=""><figcaption><p>Contextual bar UI Guide</p></figcaption></figure>

## Modals

Apps utilize modal dialogs to present information and actions to the user. Use [Contextual bars](ui-guidelines.md#contextual-bars) for more complex and involved interactions.

* Do not use modals without the app name in the tagline.
* Do not use images, such as app icons, inside the modal header.
* Do use the app name in the modal tagline.
* Do use glyph icons or simply no icons at all.

<figure><img src="../.gitbook/assets/Modals UI Guide.png" alt=""><figcaption><p>Modals UI Guide</p></figcaption></figure>

## App (bot) username

If your app has an associated bot user, the username of that user must be identical to the app name except with `-` replacing any spaces in the app name.

Eg if the app is Google Calendar app, the bot username must be _`@google-calendar`_\
Not _`@google-calendar.bot`_ or any other variation.

\
