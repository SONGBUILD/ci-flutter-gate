# ci-flutter-gate

A composite GitHub Action for one check: the tree still looks like a Flutter package.

The job fails when `pubspec.yaml` is missing, when `lib/` is missing, or when the manifest contains neither `flutter:` nor `sdk:`.

```yaml
name: ci
on: [push, pull_request]
jobs:
  gate:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: SONGBUILD/ci-flutter-gate@v1
```

`v1` is the stable tag. `@main` moves whenever this repo changes.

## License

MIT © Song Xiangrong
