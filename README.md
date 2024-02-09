# プロジェクトの作成
次のコマンドを実行すると対話式でプロジェクトを作成できる
```
npm create vue@latest
```

初めてこのコマンドを実行するとインストールが必要であることを示すログが出力されるので ```y``` と入力する。
```
> npm create vue@latest
Need to install the following packages:
create-vue@3.9.2
Ok to proceed? (y) y
```

対話式でプロジェクトの設定を作成していく。
プロジェクト名は任意の文字列でよい。
ここでは ```vue-sample-app``` としてた。
以降の内容はプロジェクトの要件に従って選択する。
特に決まっていない場合は基本的に ```No``` でよい。
```No / Yes``` の選択を変更したい場合は左右の矢印キー( ```←``` と ```→``` )で操作せよ。
```
Vue.js - The Progressive JavaScript Framework

√ Project name: ... vue-sample-app
√ Add TypeScript? ... No / Yes
√ Add JSX Support? ... No / Yes
√ Add Vue Router for Single Page Application development? ... No / Yes
√ Add Pinia for state management? ... No / Yes
√ Add Vitest for Unit Testing? ... No / Yes
√ Add an End-to-End Testing Solution? » No
√ Add ESLint for code quality? ... No / Yes

Scaffolding project in C:\Users\takum\Desktop\たこやきさん\ソースコード\02_練習(Vue)\00_HelloWorld\vue-sample-app...

Done. Now run:

  cd vue-sample-app
  npm install
  npm run dev
```

これで、プロジェクト名(例では ```vue-sample-app``` )のフォルダが作成される。

# 依存関係のインストールと動作確認
ターミナルのカウントディレクトリをプロジェクト名のフォルダへ移動する。
```
cd vue-sample-app
```

```package.json``` に記された依存関係をインストールして、動作を確認する。
```
npm install
npm run dev
```

ローカルサーバが起動されて、次の出力が確認できる
```Local``` 以降に記された
```
  VITE v5.1.0  ready in 477 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
  ➜  press h + enter to show help
```

動作結果を次に示す。
![alt text](00_動作結果.png)

```Ctrl + C``` でサーバを停止できる。

# ビルド
次のコマンドでビルドできる。
```
npm run build
```
