# Regex-Dump

Dump of regex expressions made by me for various needs

## Match YouTube links and get video id


```javascript
//str stores text containing yt link
var str = 'anytext https://youtu.be/4TPPRs1kI7U?t=1s boop';
var rgx = /https?:\/\/(?:www\.)?youtu(?:\.be\/([-A-Za-z0-9_]+)(?:\?.+)?|be\.com\/watch\?v=([-A-Za-z0-9_]+)(?:&.+)?)/g;
var arr = rgx.exec(str);
var id = arr[1] || arr[2];
console.log(id);
//id stores yt video id
```

## Match Classic Steam Keys

(From Batch Keys Activator)

```javascript
var str = 'SAS42-228BO-1488CE';
keys = str.match(/[A-z0-9]{5}(?:(?:-[A-z0-9]{5}){4}|(?:-[A-z0-9]{5}){2})/gi);
```
