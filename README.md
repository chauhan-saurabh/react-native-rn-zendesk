# react-native-rn-zendesk

Zopim Chat from Zendesk for React Native.

## Getting started

`$ npm install react-native-rn-zendesk --save`
or
`$ yarn add react-native-rn-zendesk`

### Mostly automatic installation

`$ cd ios && pod install`

### Extra steps

#### Android

Configure `ZopimChat` in `android/app/main/java/[...]/MainActivity.java`

```
ZopimChat.init("YOUR_ZENDESK_ACCOUNT_KEY").build();
```

#### IOS

Configure `ZDCChat` in `AppDelegate.m`:

```
#import <ZDCChat/ZDCChat.h>

[ZDCChat initializeWithAccountKey:@"YOUR_ZENDESK_ACCOUNT_KEY"];
```

## Usage

```javascript

In your code add `import RnZendesk from 'react-native-rn-zendesk';`.

```

ZendeskChat.startChat({
name: user.full_name,
email: user.email,
phone: user.mobile_phone,
tags: ['tag1', 'tag2'],
department: "Your department"
});

```

```
