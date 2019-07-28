# app

## Project setup
```
docker build -t vue-cli:latest .
```

### Compiles and hot-reloads for development
```
docker run -it -p 8080:8080 --rm -v "$PWD":/app vue-cli npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

### パッケージの追加について

```
docker run -it --rm -v "$PWD":/app vue-cli vue add (package name)
```

## 学んだこと

### ステートにするデータ・コンポーネントに持たせるデータ

- ステートにするデータ
    - アプリケーション全体で使い回すデータ
- コンポーネントに持たせるデータ
    - そのコンポーネントでしか使わないデータ
    - フォームの値とかドラッグ中の要素の座標・マウスポイントが要素の上に乗っているかのフラグetc...

### ミューテーション

vuex のステートを更新する時に使われる関数。基本的にこの関数を通してしか変えないこと。
また、ミューテーションの呼び出しとステートの更新を結びつけることが困難になるので、ミューテーションでは非同期処理を行ってはいけない。非同期処理はアクションで行うこと

### アクション

## 気づいたこと

- vue-cli めっちゃ便利。 Railsのscaffoldを彷彿とさせるイージーさがある。1からファイル作っていくの大変だし全部コマンド一発で作っちゃう方向でやっていこう。
    - `vue create .`: カレントディレクトリにvueプロジェクト生成
    - `vue add vuex`: vueプロジェクトにvuexを導入できる。store.js自動で作ってくれるし、読み込むコードも自動生成。神か。