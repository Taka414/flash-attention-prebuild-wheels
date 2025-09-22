# flash-attention-prebuild-wheels

## Packages

### Windows x86_64

#### Flash-Attention 2.8.3

for reForge default

| Python | Pytorch | CUDA  |
| ------ | ------- | ----- |
| 3.11   | 2.7     | 2.7.1 |

reForge version: f1.0.0v2dev-v1.10.1RC-latest-2488-ga197a41d

python: 3.11.9

torch: 2.7.1+cu128



Japanese:

reForgeのデフォルトのバージョンに対応するFlash-Attensionのwheelsが無いので自分でビルドしました。

reForgeの起動引数に「--use-flash-attention」を追記して起動すると、「Using Flash Attention」とログが出ておそらく有効化されているのかと思います。

ただし、当方所有の、RTX4080Superで生成速度に有意な差はみられませんでした。



English:

The wheels for Flash-Attention corresponding to the default version of reForge were not available, so I built them myself.

When I added "--use-flash-attention" to the startup arguments of reForge and launched it, the log displayed "Using Flash Attention," so I think it's probably enabled.

However, on my RTX 4080 Super, there was no significant difference in generation speed.



#### 導入法手順 (Japanese only)

1. リポジトリを任意のフォルダにclone

2. venv をアクティブ化

```bat
cd /d (your environment path)\webui
(your environment path)\venv\Scripts\activate
```

3. pipでインストール

```bat
pip install (your download path)\flash_attn-2.8.3-cp311-cp311-win_amd64.whl
```

4. 導入できたかチェック

```bat
pip show flash-attn
- - - - - - - - - -
Name: flash_attn
Version: 2.8.3
Summary: Flash Attention: Fast and Memory-Efficient Exact Attention
Home-page: https://github.com/Dao-AILab/flash-attention
Author: Tri Dao
Author-email: tri@tridao.me
License:
Location: ********\venv\Lib\site-packages
Requires: einops, torch
Required-by:
```

5. 起動引数に「--use-flash-attention」を追記して起動





