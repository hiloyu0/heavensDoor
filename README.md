# かおほん

顔を検知して、その顔を本のようにひらく演出アプリです。カメラ（リアルタイム）、写真、見本の顔で試せます。

- 公開ページ: https://hiloyu0.github.io/kaohon/
- 顔認識: [@vladmandic/face-api](https://github.com/vladmandic/face-api)（MIT）のモデルを `model/` に同梱
- 見本の顔: [vladmandic/human](https://github.com/vladmandic/human)（MIT）のサンプル画像のうち CGI のもの（実在の人物ではありません）
- 描画: three.js r128
- 顔と髪の認識: [MediaPipe Tasks Vision](https://github.com/google-ai-edge/mediapipe)（Apache-2.0）の Face Landmarker と Hair Segmenter を `mp/` に同梱（読み込めないときは face-api に切り替え）
