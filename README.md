# things-button

## This component provides the style of the button, whether to display the confirmation window when the button is clicked, the title and message setting function of the confirmation window.


Example:

```html
<things-button
     id="button-id"
     color="indigo"
     confirm=true
     title="Confirm"
     message="This is message field">
     Button name
</things-button>
```


# things-button-bar
## It is a button bar that manages several buttons. If the screen is 800px or less, it will be displayed in the form of things-button-group, that is, a fab icon.
###  Example
    var buttons = [{
      id: 'import',
      text: 'import',
      icon: 'icons:import'
    }, {
      id: 'export',
      text: 'export',
      icon: 'icons:export'
    }, {
      id: 'add',
      text: 'add',
      icon: 'icons:add'
    }, {
      id: 'delete',
      text: 'delete',
      icon: 'icons:delete'
    }, {
      id: 'save',
      text: 'save',
      icon: 'icons:save'
    }];
    ...
    <things-button-bar id="btn-bar" buttons="[[buttons]]"></things-button-bar>
    ...
    listeners: {
      'btn-bar.things-button-tap' : 'onTapButton'
    },
    ...
    onTapButton: function(e) {
      console.log(e);
    }


# things-button-group
## It provides the function to represent the group of buttons that manage several buttons in the form of a fab icon.
### Example
    var buttons = [ {
      id: 'import',
      text: 'import',
      icon: 'icons:import'
    }, {
      id: 'export',
      text: 'export',
      icon: 'icons:export'
    }, {
      id: 'add',
      text: 'add',
      icon: 'icons:add'
    }, {
      id: 'delete',
      text: 'delete',
      icon: 'icons:delete'
    }, {
      id: 'save',
      text: 'save',
      icon: 'icons:save'
    } ];
    ...
    <things-button-group id="btn-group" buttons="[[buttons]]"></things-button-group>
    ...
    listeners: {
      'btn-group.things-button-tap' : 'onTapButton'
    },
    ...
    onTapButton: function(e) {
      console.log(e);
    }

## 2. Development
### 2.1 Install Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

### 2.2 Run Application

```
$ polymer serve
```

### 2.3 Build Application

```
$ polymer build
```

You can launch the server from `build/bundled` or `build/unbundled` with the following command:

```
$ polymer serve build/bundled
```

### 2.4 Run Tests

```
$ polymer test
```

The test has been set up as described in [web-component-tester](https://github.com/Polymer/web-component-tester).
You can run the test with the following command.
```
$ polymer test
```
