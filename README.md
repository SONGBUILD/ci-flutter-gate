# ci-flutter-gate

A composite GitHub Action that fails the job when a Flutter tree is missing `pubspec.yaml` or `lib/`.

```yaml
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
