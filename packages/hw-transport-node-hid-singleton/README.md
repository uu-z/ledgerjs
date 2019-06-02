<img src="https://user-images.githubusercontent.com/211411/34776833-6f1ef4da-f618-11e7-8b13-f0697901d6a8.png" height="100" />

[Github](https://github.com/LedgerHQ/ledgerjs/),
[Ledger Devs Slack](https://ledger-dev.slack.com/)

## @ledgerhq/hw-transport-node-hid-singleton

Allows to communicate with Ledger Hardware Wallets.

**[Node]**/Electron **(HID)** – uses `node-hid` and `usb-detection`. Keep transport opened and re-use it as a singleton, one device at a time on a computer but more robust implementation.

## API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

-   [TransportNodeHidSingleton](#transportnodehidsingleton)
    -   [Examples](#examples)
    -   [isSupported](#issupported)
    -   [list](#list)
    -   [listen](#listen)
        -   [Parameters](#parameters)
    -   [disconnect](#disconnect)
    -   [open](#open)

### TransportNodeHidSingleton

**Extends TransportNodeHidNoEvents**

node-hid Transport implementation

#### Examples

```javascript
import TransportNodeHid from "@ledgerhq/hw-transport-node-hid-singleton";
...
TransportNodeHid.create().then(transport => ...)
```

#### isSupported

#### list

#### listen

##### Parameters

-   `observer` **Observer&lt;DescriptorEvent&lt;any>>** 

Returns **Subscription** 

#### disconnect

globally disconnect the transport singleton

#### open

if path="" is not provided, the library will take the first device

Returns **[Promise](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[TransportNodeHidSingleton](#transportnodehidsingleton)>** 