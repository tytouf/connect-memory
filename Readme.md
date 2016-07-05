
**connect-memory** is the original memory session store for Connect.

Setup
-----

```sh
npm install connect-memory express-session
```

Pass the `express-session` store into `connect-memory` to create a `MemStore` constructor.

```js
var session = require('express-session');
var MemStore = require('connect-memory')(session);

app.use(session({
    store: new MemStore(options),
    secret: "shushhhh it's a secret"
}));
```

License
=======

MIT
