# ReadMe
RailsとLaravelの教材執筆時の手順書です。

完全に自分用に書いているので、読みにくい部分があると思います。

自分で執筆する前提だったので、手順書の時点で結構説明まで書いています。

主に以下のフォーマットで書いていました。

手順書ファイルは`○章.md`

```
## 項のタイトル

(任意：実装時に参考にした記事等あればURLを記載)

何をやるか簡単に説明

コード編集 or コマンド (コードブロックで記載)

コマンドの実行結果
```
- 記載例
````
## laravel/uiの導入

参考：https://blog.hrendoh.com/laravel-6-setup-bootstrap4-with-laravel-ui/#Bootstrap_4.md`

laravel/ui を導入します。

次のコマンドを実行してください。
```console
composer require laravel/ui "1.x" --dev
```

コマンドを実行すると次のようなメッセージが表示されます。
```console
・
・
・
  - Installing laravel/ui (v1.3.0): Downloading (100%)
・
・
・
Package manifest generated successfully.
64 packages you are using are looking for funding.
Use the `composer fund` command to find out more!
```
````

上記の手順から最終的に以下のように執筆しました。

- [laravel-fashion-ec-app-curriculum/2-2 Bootstrapを導入しよう.md at master · Techpit-Contents/laravel-fashion-ec-app-curriculum](https://github.com/Techpit-Contents/laravel-fashion-ec-app-curriculum/blob/master/2%E7%AB%A0%20%E5%95%86%E5%93%81%E4%B8%80%E8%A6%A7%E7%94%BB%E9%9D%A2%E3%82%92%E5%AE%9F%E8%A3%85%E3%81%97%E3%82%88%E3%81%86/2-2%20Bootstrap%E3%82%92%E5%B0%8E%E5%85%A5%E3%81%97%E3%82%88%E3%81%86.md#laravelui%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB)

コマンド実行やコード編集箇所などは手順書の時点でコードブロックで記述しておくと、執筆時コピペで済むので楽です。

コード編集箇所は`diff:ファイルパス`まであらかじめ設定しておきます。

````
```diff:package.json
{
    "devDependencies": {
        ・
        ・
        ・
-    }
+    },
+    "dependencies": {
+        "@fortawesome/fontawesome-free": "^5.15.1"
+    }
}
```
````

## その他

- 代筆者も動作確認は必要だと思うので、どうなれば正しく動作しているかがわかるように、動作確認時のスクショ等は手順書に載せてもらう必要があるかと思います。

- 実装物は章ごとにブランチを分けると、動作確認がしやすくなると思います。

- 参考までに、1章あたり3日で執筆してました。代筆の場合はキャッチアップ込なので、より日数かかると思います。
     
