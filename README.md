# flash-attention-prebuild-wheels

## Packages

### Windows x86_64

#### Flash-Attention 2.8.3

for reForge default

| Python | Pytorch | CUDA  |
| ------ | ------- | ----- |
| 3.11   | 2.7     | 2.7.1 |
|        |         |       |
|        |         |       |

reForge version: f1.0.0v2dev-v1.10.1RC-latest-2488-ga197a41d

python: 3.11.9

torch: 2.7.1+cu128



Ja:

reForgeのデフォルトのバージョンに対応するFlash-Attensionのwheelsが無いので自分でビルドしました。

reForgeの起動引数に「--use-flash-attention」を追記して起動すると、「Using Flash Attention」とログが出ておそらく有効化されているのかと思います。

ただし、当方所有の、RTX4080Superで生成速度に有意な差はみられませんでした。



En:

The wheels for Flash-Attention corresponding to the default version of reForge were not available, so I built them myself.

When I added "--use-flash-attention" to the startup arguments of reForge and launched it, the log displayed "Using Flash Attention," so I think it's probably enabled.

However, on my RTX 4080 Super, there was no significant difference in generation speed.