# libpng
GNU Emacs30.0.50に含まれる`java/INSTALL`にしたがって取得したlibpngモジュールのレポジトリ。

# 作成した手順

1. [Google Gitのlibpng](https://android.googlesource.com/platform/external/libpng/)をclone


```bash
$: git clone https://android.googlesource.com/platform/external/libpng/
```

2. `nougat-release`ブランチから修正用ブランチ`my/nougat-release`をcheckout

```bash
$: cd libpng
$: git checkout nougat-release
$: git checkout -b my/nougat-release
```

3. 空レポジトリにpush

```bash
$: git add -A
$: git commit -m 'nanika commit messages...'
$: gh repo create my-libpng --public
$: git remote add mine https://github.com/JIBUN/my-libpng.git
$: git branch -M my/nougat-release
$: git push -u mine my/nougat-release
```
