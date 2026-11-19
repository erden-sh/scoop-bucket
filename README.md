# Erden Scoop bucket

The [Scoop](https://scoop.sh) manifest for [Erden](https://erden.sh)'s command line tool, `erden` (also available as
`den`), which checks, packs and publishes ontology projects. The tool's source is in
[erden-sh/erden](https://github.com/erden-sh/erden).

```powershell
scoop bucket add erden https://github.com/erden-sh/scoop-bucket
scoop install erden
```

The manifest installs the Windows x64 release archive, which carries the Node.js runtime and both engines the tool
runs on. For tab completion in PowerShell, add `erden completions powershell | Out-String | Invoke-Expression` to your
`$PROFILE` (releases after 0.1.0).

`bucket/erden.json` is written from the release's pinned archive digest by `release/write-package-manifests.mjs` in
erden-sh/erden, and its release workflow pushes it here after each release installs and runs on every platform. Its
`checkver` and `autoupdate` let Scoop's own tools follow new releases too. Please don't edit it by hand: open an issue
in [erden-sh/erden](https://github.com/erden-sh/erden/issues) instead.

## License

Apache License 2.0 (see [LICENSE](LICENSE)); the copyright holder is Ingenio Ventures Inc. "Erden" is a trademark of
Ingenio Ventures Inc.
