# things-button

## 이 컴포넌트는 버튼의 스타일, 버튼을 클릭했을 때 확인창 표시 여부, 확인창 타이틀 및 메시지 설정 기능 등을 제공한다.


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
## 이는 여러 개의 버튼들을 관리하는 버튼 바이다. 만약 화면이 800px 이하이면 things-button-group, 즉 fab icon 형태로 표현한다.
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
## 여러 개의 버튼들을 관리하는 버튼 그룹을 fab icon 형태로 표현하는 기능을 제공한다.
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

## 2. 개발
### 2.1 Polymer-CLI 설치

먼저 [Polymer CLI](https://www.npmjs.com/package/polymer-cli)가 설치되어 있는지 확인한다. 다음, `polymer serve`를 실행하여 로컬에서 응용 프로그램을 제공한다.

### 2.2 Application 실행

```
$ polymer serve
```

### 2.3 Application 빌드

```
$ polymer build
```

아래 명령어로 `build/bundled`나 `build/unbundled`에서 서버를 띄울 수 있다.

```
$ polymer serve build/bundled
```

### 2.4 Tests 실행

```
$ polymer test
```

[web-component-tester](https://github.com/Polymer/web-component-tester)에서 설명한 대로, 테스트 설정은 이미 완료되어 있다.
아래 명령어로 테스트를 실행할 수 있다.
```
$ polymer test
```
