Chat++ Change Logs
=================
## 5.0.0
* Chat++ is rewritten in [ECMAScript 6](http://www.ecma-international.org/publications/standards/Ecma-262.htm),
 transformed by [babel](https://babeljs.io/), built by [gulp](http://gulpjs.com/).
 Refer the [Contribution Guidelines](./CONTRIBUTING.md) file for more information.
* Emoticon Data File Structure changed. The `regex` field is not necessary anymore. (However, you can add it if you want)
```
// Before
"emoticons": [
    {"key": "(rofl2)", "regex": "\\(rofl2\\))", "src": "https://i.imgur.com/UD2NE5U.gif"},
]

// From 5.0.0
"emoticons": [
    {"key": "(rofl2)", "src": "https://i.imgur.com/UD2NE5U.gif"},
]
```

* New mention methods. Use `@admin` to mention all room's admins,
use `@random` to randomly mention a member inside the room.
* No longer show error messages when there are some emoticon data that can not be loaded.
Display a `ERRORS` text next to the Emoticon text instead.
* Immediately turn on or off emoticons when toggle the `E` button in the Chat toolbar.


## 4.3.2
* Fix bug with "new" text in Chat++ icon

## 4.3.1
* Fix bug with sending message by Shift + Enter

## 4.3.0
* Disabled Desktop Notification Feature (base on registered rooms)
* Quick Title Tag, Quick Info Tag
~~~
    ```
    ``` => tag [code][/code] (default)

    ``i
    ``` => tag [info][/info]

    ``t
    ``` => tag [title][/title]
~~~
* Change emoticon alt attribute value (From only emoticon text to emoticon text plus emoticon data name)
From now, you can check the emoticon data that an emoticon belongs to by hovering the mouse over the emoticon
* Display a notification text (**new**) inside the Chat++ icon when Chat++ is updated

## 4.2.0
* Display detailed error when can not load or parse Emoticons data in both Emoticons page and Chatwork
* Rewrite Emoticons data loading flow. Now if there are errors with Emoticons data files, only that data will be disabled. Chat++'s features, including emoticon, will still work
(In previous versions, failing in loading or parsing Emoticons data file will cause Chat++ become unable to work)
* Display confirmation alert when clicking at "Reset" button in Emoticons page
* Display countdown message before Chat++ is loaded
* Bug fix

## 4.1.0
* Code Highlight: Support more languages
* Support specifying the language of the code
* Code block will be applied word wrap by default. Support "nowrap" option
Example
```
ruby
#ruby code, long text is wrapped by default
puts "This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text"
```

```
ruby nowrap
#ruby code, do not wrap long text
puts "This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text. This is a super long text"
```
* Use dark theme for code highlight
* Thumbnail feature is OFF by default. Please turn it on if you want to use it.
* Thumbnail size (height) is rescaled from 150px to 125px
* Display gyazo's https image thumbnail
* Show thumbnail in Task view, as well as in Chat room description
* Now, many Chat++ features such as external emoticons, code highlight, thumbnail display ... will be automatically applied after loading Chatwork
(In previous versions, you must switch room to make everything become effective)

## 4.0.0 - Big Update
* View list issues at [Version Four Milestone](../../milestones/Version%20Four)
* Highlight Code
* Display image thumbnail. Support direct image link, gyazo link, Facebook image link ...
* Many new Shortcuts that help users to quickly switch Chat room.
    *  Go to the first Room in the list
    *  Go to the first nonstick Room in the list
    *  Go to the Room below in the list
    *  Go to the Room above in the list
    *  Go to the first Room that has new unread Message(s)
    *  Go to the first Room that has new unread Mention Message(s)
* New setting page
* New change logs page
* New feature list page
* Update Emoticons page. It is now easier to arrange data priority
* Bug Fixes.

## 3.0.2
* Fix bug with room title

## 3.0.1
* Add Vietnamese Emoticon Data

## 3.0.0 - Big Update
* View list issues at [Happy Birthday Release Milestone](../../milestones/Happy%20Birthday%20Release)
* Room Shortcut Feature Added.
* Mention Jump Feature Added.
* Drop OFFENSIVE mode.
* Allow users to reply their own message.
* Add room info button.
* Several Bug Fixes. 

## 2.0.0 - Big Update
* View list issues at [Happy Lunar New Year Release Milestone](../../milestones/Happy%20Lunar%20New%20Year%20Release)
* Mention syntax changed. (use `_` for omitting username, use `.` for picon)
* Mention users that are in friend list, but not present in Chat box (using `@#`)
* Register Groups name and members. Mention Group.
* Shortcut Feature Added.
* Several Bug Fixes.

## 1.0.3
* Add Skype data to official list
* Fix bug with mention popup

## 1.0.2
* Add official emoticons data list in option page
* Temporarily remove change log

## 1.0.1
* Mention user with Nickname.
* Fix bug: Can not initialize Default Emoticons Data at the first load.
* Fix bug: Two emoticons data have the same priority.

## 1.0.0
* Change version for release purpose.
* View list issues at [Happy New Year Release Milestone](../../milestones/Happy%20New%20Year%20Release)

## 0.1.3
* Fix bug with arrows inputted
* Apply multiple emoticons data

## 0.1.2
* Fix bug with `version_type` in Manifest

## 0.1.0
* Add secret emoticons

## 0.0.9
* Add `@_all` and `@__all` feature
* Add `@_me` and `@__me` feature

## 0.0.8
* Add `@me` feature
* Add `@all` feature
* Add show picon only when type `@__`
* Add show TO and picon only when type `@_`
* Move popup to left when is hidden

## 0.0.7
* Press ESC don't hide the pop up
* Send message when choose press Enter to send setting

## 0.0.6
* Now It is possible to change Mention Status from popup page. The status is sync via google account like Emoticon Status.

## 0.0.5
* Reverse emoticons change logs order in option page.
* Add button to turn ON/OFF Mention Feature.