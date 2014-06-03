require-test-case
=================

This is a test case to reproduce a bug in requirejs 2.1.11.
https://github.com/jrburke/requirejs/issues/1112

To observe the issue

```
git clone https://github.com/xzyfer/require-test-case.git
cd require-test-case
make
```

Then open your browser to `localhost:3000`

### Expected output

```
loaded
foo-1
foo-2
```

### Observed output

```
loaded
foo-1
Uncaught Error: Load timeout for modules: bar/baz
http://requirejs.org/docs/errors.html#timeout
```
