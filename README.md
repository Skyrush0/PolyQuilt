# PolyQuilt
---
PolyQuiltはローポリモデリングをサポートするBlender2.8用アドオンです。シンプルでオーソドックスでオールドスクールな面張り機能に加えてドラッグや長押し等のマウスオペレーションに様々な機能を割り振ることでツールの切り替えを最小限にしてポリゴンモデリングに没頭する事を可能にします。

# β版について

ダウンロードは[こちら](https://github.com/sakana3/PolyQuilt/releases)から

現在、Blender2.8はβテスト中の為、幾つかの不具合や実装待ち項目があります。本アドオンを利用したことによるデータの破損などは責任を持ちません。フィードバックはこちらの[Issues](https://github.com/sakana3/PolyQuilt/issues)かTwitterアカウント[sakana3](https://twitter.com/sakanaya) まで宜しくお願い致します。

特にこのアドオンを実際に利用したモデリング過程で感じた違和感やストレスなどお気軽にフィードバック頂けるとPolyBuildのより良い発展に繋がります。

## 既知の不具合

- とても重いです。一応対応の目途は立っていますが今のところは我慢して１オブジェクト5000ポリゴンぐらいのものにお使いください。あまり大きなポリゴン数のものに適用するとBlenderが固まり操作不能になる恐れがありますのでご注意ください。

# 導入方法

[こちら](https://github.com/sakana3/PolyQuilt/releases)よりダウンロードして編集→設定→アドオン→インストールよりインストールしてください。インストールした段階ではまだ使えませんのでその後検索バーよりPolyQuiltを検索しチェックボックスをOnにしてください。

編集モードに入るとPolyBuildの下にアイコンが追加されているのでこれをクリックでPolyQuiltがアクティブツールになります。

# 機能一覧

## 操作早見表 

||クリック|ドラッグ|長押し|長押し後ドラッグ|
|:-:|:-:|:-:|:-:|:-:|
|空間|[頂点作成](#頂点作成)→[面張り](#面張り)||[削除/融解](#削除/融解)|[ナイフ](#ナイフ)||
|点|[面張り](#面張り)|[移動(結合)](#移動)|[削除/融解](#削除/融解)||
|辺|[頂点挿入→面張り](#面張り)|[移動](#移動)|[削除/融解](#削除/融解)|[ループカット](#ループカット)|
|面||[移動](#移動)|[削除](#削除/融解)||


## 移動  

点、線、面の上でマウスドラッグでビュー平面状の移動ができます。エッジの頂点は別エッジの頂点に近づける事で結合する事ができます。

## 頂点作成

何もない空間をクリックで頂点が作成されます。通常はそのまま面張りモードになりますがジオメトリを点モードにすれば連続で点を作れます。

## 面張り

何もないエリアか点の上でクリックで面張りを開始します。クリックする度に点、線、面が追加されます。最後に配置した点の上でクリック(ダブルクリックと同意)か右クリックで終了しまた新たな面を作ることができます。

画面上部のツールメニューより作成するジオメトリを点、線、三角形、四角形、ポリゴンから選ぶ事ができます。

また同一面の頂点でクリックすると面の分断になります。  

## 削除/融解

点、線、面の上で長押しでその要素を消去or融解します。共有する線や面がある場合は融解、そうでない場合は削除になります。

## ナイフ

空間で長押し後にドラッグでナイフを実行できます。

## ループカット

辺の上で長押し後ドラッグで辺をループカットできます。

# 環境設定

ドキュメント準備中

# 実装予定

- [ ] ワイヤーカット
- [ ] 分離(Rip)
- [ ] 左右対称
- [ ] LoopCutの末端三角形対応
- [ ] 選択
- [ ] ハンドリトポ編集
