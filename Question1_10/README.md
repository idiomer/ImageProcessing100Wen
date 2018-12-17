# 問題 1~10

## 問題1. チャネル入れ替え

画像を読み込み、RGBをBGRの順に入れ替えよ。

画像の赤成分を取り出すには、以下のコードで可能。
cv2.imread()関数ではチャネルがBGRの順になることに注意！
これで変数redにimori.jpgの赤成分のみが入る。

```python
import cv2
img = cv2.imread("assets/imori.jpg")
red = img[:, :, 2].copy()
```

|入力画像|出力画像|
|---|---|
|![](../assets/imori.jpg)|![](answer_1.jpg)|

## 問題2.

画像をグレースケールにせよ。
グレースケールとは画像の輝度表現方法の一種であり、下式で計算される。

Y = 0.2126 R + 0.7152 G + 0.0722 B

|入力画像|出力画像|
|---|---|
|![](../assets/imori.jpg)|![](answer_2.jpg)|