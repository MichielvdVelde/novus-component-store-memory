# novus-component-store-memory

In-memory key/value store for [novus-component](https://github.com/MichielvdVelde/novus-component).
This module is included by default when `npm install`ing the `novus-component@>=2.1.0` module.

Despite the fact that it was designed to be used by `novus-component`, you can install
and use this module independently if so desired.

# Usage

Install using `npm`:

```
npm i novus-component-store-memory
```

Setting it up:

```js
import { MemoryStore } from 'novus-component-store-memory';

const store = new MemoryStore();
```

Getting a key:

```js
// MemoryStore.get(key, def = null)
let value = store.get('key', false);
// 'value' is false if there was no such key found
```

Setting a key:

```js
// MemoryStore.set(key, value, override = true)
store.set('key', 'value');
```

## License

Copyright 2016 Michiel van der Velde.

This software is licensed under the [MIT License](LICENSE)
