# spawn
 [co](https://github.com/tj/co)-like function that work in the browser

 inspired by https://jakearchibald.com/2014/es7-async-functions/

# Install

with bower:

    bower install spawn

# Example

```js
spawn(function* () {
  const result = yield Promise.resolve(true);
  return result;
}).then(function (value) {
  console.log(value);
}, function (err) {
  console.error(err);
});
```
