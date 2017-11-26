Node Jdownloader API
======
**A NodeJS wrapper for My.jdownloader.org API**

https://my.jdownloader.org/developers/

This is a rewritten version of this PHP wrapper
https://github.com/tofika/my.jdownloader.org-api-php-class

Features
--------
- Connect to the My.JDownloader service
- Disconnect from the My.JDownloader service
- List Devices
- Add Links and start download

Usage
--------

To install `jdownloader-api` in your node.js project:

```
npm install jdownloader-api
```

And to access it from within node, simply add:

```javascript
const jdownloaderAPI = require('./jdownloaderAPI');
```
API
--------
## Connect

```javascript
jdownloaderAPI.connect(_USERNAME_, _PASSWORD_)
```

## Disconnect

```javascript
jdownloaderAPI.disconnect()
```

## listDevices

```javascript
// List all active devices from the connected account
// deviceName and deviceId
jdownloaderAPI.listDevices()
```

## addLinks

```javascript
// This will add links to the device and autostart downloads
// nb : links must be comma separated
jdownloaderAPI.addLinks(LINKS, DEVICEID)
```