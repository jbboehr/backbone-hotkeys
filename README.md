#About
**Backbone Hotkeys** is an extension to the vanilla Backbone View which lets you easily add and remove handlers for keyboard events supporting almost any key combination.  Uses the *hotkey.js* library written by: [John Resig](http://github.com/jeresig/jquery.hotkeys) as a base, which was based off of the plugin by Tzury Bar Yochay: [jQuery.hotkeys](https://github.com/tzuryby/jquery.hotkeys)

## Demo
[Demo](http://htmlpreview.github.com/?https://github.com/rpocklin/backbone-hotkeys/master/example/index.html)

## Types
Supported types are `'keydown'`and `'keyup'`.

## How-to
Include *hotkeys.js* and *backbone-hotkeys.js* after *backbone.js* in your app.

## Example

    App.SomeView = Backbone.View.extend({
      el:$('#some-id'),

      events:{

        'keyup[esc]       body': 'someMethod',  // hotkeys keymapping
        'keyup[Alt+m]     body': 'someMethod',  // hotkeys keymapping
        'keyup[Ctrl+left] body': 'someMethod'   // hotkeys keymapping
      }
    });


## Notes
TBD.

## Compatibility
Works with jQuery 1.7.2 and 1.8.3 and Backbone 0.9.2.
