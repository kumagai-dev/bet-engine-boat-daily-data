# BET ENGINE — BOAT RACE Daily Data

このRepositoryは、公開BET ENGINE画面が読み込む**表示専用の軽量Prediction Dataset**だけを配信します。モデルRepositoryではありません。

## 公開するもの

各日付のVersioned JSON、公開Manifest、最新Datasetへの参照だけを公開します。JSONには画面に表示する会場・レース番号・AI本命艇・表示用確率・上位候補・表示用判定・結果・答え合わせ・JST生成時刻を含めることがあります。

## 公開しないもの

Frozen Model、Feature State、feature_v2内部データ、Calibration、Reliability内部Dataset、OOF、全120通りParquet、Private Worker Source、Token、Secret、Credential、Private Repository URLは一切含めません。

## 公開状態

DatasetはPrivate Prediction WorkerがIntegrity検証に成功した後だけ、Versionedファイルを先に公開し、その後に公開Manifestの参照を切り替えます。公開失敗時は既存の最新Datasetを維持します。

This repository contains public display data only. It does not contain BOAT RACE models, features, internal artifacts, or credentials.
