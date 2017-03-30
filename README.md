# things-button

## 버튼의 스타일과 버튼을 클릭했을 때 확인 창 표시 여부 및 확인 창 타이틀, 메시지 설정 기능 제공


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
##

## 2. 개발
### 2.1 Polymer-CLI 설치

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

### 2.2 Application 수행

```
$ polymer serve
```

### 2.3 Application 빌드

```
$ polymer build
```

아래 명령어로 ` build/bundled`나 ` build/unbundled`에서 서버를 띄울수 있다.

```
$ polymer serve build/bundled
```

### 2.3 Running Tests

```
$ polymer test
```

테스트는 [web-component-tester](https://github.com/Polymer/web-component-tester)에서 설명한데로 설정완료됨.
아래 명령어로 테스트를 수행할 수 있다.
```
$ polymer test
```
