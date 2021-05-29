Gio CJK font tool

> credits to https://git.sr.ht/~eliasnaur/font

## Dev

1. Install `fonttools` first.

2. Make font subset

```console
pyftsubset SourceHanSansSC-Regular.ttf  --unicodes="U+0020-007F,u+8f6c,u+6362,u+5668" --output-file="ttfs/subset.ttf"
```

3. Generate go module

```console
go run gen.go
```

## Ref
- Creating font subsets https://markoskon.com/creating-font-subsets/
- https://github.com/tailscale/tailscale-android/blob/db13aa4e92cca966242bc84ad138b34fff29a493/cmd/tailscale/ui.go#L171