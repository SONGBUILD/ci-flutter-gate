# ci-flutter-gate

Reusable **GitHub Action** that checks a Flutter-shaped tree: required files exist.

On D9 this becomes its own public repo. Other repos can later `uses: SONGBUILD/ci-flutter-gate@v1` — not wired today.

```yaml
jobs:
  gate:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: SONGBUILD/ci-flutter-gate@main
```

## License

MIT © Song Xiangrong
