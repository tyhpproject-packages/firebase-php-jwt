<!-- tyhp-readme:start -->
# tyhpdef/firebase-php-jwt

Tyhp type definitions for `firebase/php-jwt` `7.1.1`.

```bash
composer require --dev tyhpdef/firebase-php-jwt:7.1.1
```

This is a metapackage. Composer also installs `tyhpdef/firebase-php-jwt-impl` (type files).
Require **this** name, not `tyhpdef/firebase-php-jwt-impl`.

See https://tyhplang.com.

## Maintain `firebase/php-jwt`? Ship the types yourself

If you are a Packagist maintainer of `firebase/php-jwt`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/firebase-php-jwt-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `firebase/php-jwt` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/firebase-php-jwt": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `firebase/php-jwt` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `firebase/php-jwt` with a real constraint,
   `"replace": { "tyhpdef/firebase-php-jwt": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `firebase/php-jwt` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/firebase-php-jwt` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
