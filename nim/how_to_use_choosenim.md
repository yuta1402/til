# How to install choosenim
## Install choosenim

```
$ curl https://nim-lang.org/choosenim/init.sh -sSf | sh
choosenim-init: Downloading choosenim-0.3.2_linux_amd64
    Prompt: Can choosenim record and send anonymised telemetry data? [y/n]
        ... Anonymous aggregate user analytics allow us to prioritise
        ... fixes and features based on how, where and when people use Nim.
        ... For more details see: https://goo.gl/NzUEPf.
    Answer: y
```

上記でインストール後、$HOME/.nimble/binを$PATHに通すように言われるので、次の行を.bashrcに追加。

```
export PATH=$HOME/.nimble/bin:$PATH
```

これで、最新版のNimがインストールされる。

## References
- https://nim-lang.org/install_unix.html
- https://github.com/dom96/choosenim
