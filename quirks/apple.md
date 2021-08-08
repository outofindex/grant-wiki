
## Generate Client Secret

```js
var jws = require('jws')

exports.sign = ({client_id, key_id, team_id, private_key}) => {
  var epoch = Math.floor(new Date().getTime() / 1000)

  var options = {
    header: {
      typ: 'JWT',
      alg: 'ES256',
      kid: key_id,
    },
    payload: {
      iss: team_id,
      sub: client_id,
      aud: 'https://appleid.apple.com',
      iat: epoch,
      exp: epoch + (60 * 60 * 24), // 1 day, up to 180 days
    },
    secret: private_key
  }

  return jws.sign(options)
}
```
