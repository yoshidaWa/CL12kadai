# 左右反転画像 生成プログラム flip.py

## 1.概要
引数で指定した画像の左右反画像を作成するphthon3で動作するプログラムです。

## 2.ソースコード
```
python
# このプログラムはpython3用です。
# あらかじめ　pip install pillow で pillow をインストールしておきます。
from PIL import Image
import sys

# コマンドライン引数から入力画像と出力画像のファイル名を取得
input_image = sys.argv[1]
output_image = sys.argv[2]

# 画像の読み込み
img = Image.open(Image.FLIP_LEFT_RIGHT)

# 画像の保存
img_flip.save(output_image)
# 左右反転画像　生成プログラム　flip.py
```

## 3.使い方
### 3.1.実行例
- コマンドラインフォーマット

```
python3 flip.py <imput_image_path><output_image_path>
```

- 利用例

```
python3 flip.py input.jpg output.jpg
```
### 3.2.出力例
- 以下のように入力画像の左右反転画像が表示されます。

| 入力画像(input.jpg) | 出力画像(output.jpg) |
| --- | --- |
| <img width="907" height="605" alt="input" src="https://github.com/user-attachments/assets/ad10c8c9-bad3-4e35-8bbd-603d53b6a290" /> | <img width="907" height="605" alt="output" src="https://github.com/user-attachments/assets/35e7f153-bc5f-45fe-a66d-e0bb84a87896" />
 |

 以上
