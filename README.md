# step

`step()` は `lmer` や `glmer` で作られたモデルを項に取った後、
Backward Elimination で作成されたモデルをリストとして返します。

## Prerequisite

`lme4`と`devtools`パッケージが必要です。

```R
install.packages("lme4")
install.packages("devtools")
```

## how to use

`devtool` に含まれる `install_github` 関数を使い、Github のリポジトリからインストールします。

:snake: WindowsとMacでの動作は未確認です。

```R
require(lme4)
require(devtools)
install_github("kisyaman/step")
require(step)

# 検証したいモデルの最大モデルを組む
model = model
#
models = step(model,beeping=T)

```

## 質問

[issue](https://github.com/kisyaman/step/issues)をご利用ください。

## License
MIT
