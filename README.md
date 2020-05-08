# test-git-patch

## Applying a patch with `git apply`
To apply the diff:
`cd` into the directory containing lodash.js then run this:
```
git apply p.patch
```

Another way to do it where you specify the location (directory) containing lodash.js is like this...
First, `cd` somewhere other than a directory containing lodash.js.
Then, run this:
```
git apply p.patch
```

## Applying a patch with `patch`
```
patch <path-to-file-you-want-to-patch> <path-to-patch-file>
```

Note that it seems like `patch` does not like `..` in the paths.
