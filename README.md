# test-git-patch

## Specific to this repo
From the root:
```
git apply --directory=to-patch p.patch
```

or (if you want to use a fully qualified path):
```
git apply --unsafe-paths  --directory=$(pwd)/to-patch p.patch
```


## More Generically

### Applying a patch with `git apply`

Note that `git-apply` is sub-optimal in that it doesnt give you and error when the action doesn't work.

To apply the diff:
`cd` into the directory containing lodash.js then run this:
```
git apply p.patch
```

### Applying a patch with `patch`
```
patch <path-to-file-you-want-to-patch> <path-to-patch-file>
```

Note that it seems like `patch` does not like `..` in the paths.
