# hap

## IntelliSense

Char **→** refers to the `TAB` key

#### Tag

1. In the page file, enter `h-` to prompt the shortcut template fragment. The supported template fragments are as follows:

| Trigger       | Content                |
| ------------: | ---------------------- |
| `h-app→`      | Creates a hap app      |
| `h-page→`     | Creates a hap page     |
| `h-import→`   | Creates a hap import   |
| `h-template→` | Creates a hap template |
| `h-style→`    | Creates a hap style    |
| `h-script→`   | Creates a hap script   |

**Example**

Trigger: `h-import→`

```html
<import name='' src=''></import>
```

2. In `<template>`, enter `h-` to prompt the supported components

**Example**

Trigger: `h-div→`

```html
<div></div>
```

#### Attributes

In the start tag of the component, enter the space bar to prompt the attributes supported by the component

**Example**

Trigger: `<div `

![](https://image.ibb.co/n6ptA7/Intelli_Sense1.png)

## Emmet snippets

#### Style

**Example**

Trigger: `h-font-weight→`

```html
font-weight: normal;
```

#### Import Module

The shorthand way of importing the module is the same as the sample code in the document

**Example**

Trigger: `h-@system.router→`

Content:

```javascript
import router from '@system.router'
```

#### Interface

The abbreviation of the interface is the same as the interface definition in the document

**Example**

Trigger: `h-storage.set→`

Content:

```javascript
storage.set({
  key: 'key',
  value: 'value',
  success: function (data) {
    console.info('success');
  },
  fail: function (data, code) {
    console.info('fail');
  },
  complete: function () {
    console.info('complete')
  }
})
```

Since the framework supports system sharing and three-party sharing, in order to avoid duplication of names. The interface is as follows:

Trigger: `h-system.share.share→`

Content:

```javascript
share.share({
  type: 'text/html',
  data: '<b>bold</b>',
  success: function (data) {
    console.info('success')
  },
  fail: function (data, code) {
    console.info('fail')
  },
  cancel: function (data) {
    console.info('cancel')
  },
  complete: function () {
    console.info('complete')
  }
})
```

Trigger: `h-service.share.share→`

Content:

```javascript
share.share({
  shareType: 0,
  title: 'title',
  summary: 'summary',
  imagePath: 'xxx/xxx/xxx/share.jpg',
  targetUrl: 'http://www.example.com',
  success: function (data) {
    console.info('success')
  },
  fail: function (data, code) {
    console.info('fail')
  },
  cancel: function () {
    console.info('cancel')
  }
})
```

## Installation

npm install && npm run compile