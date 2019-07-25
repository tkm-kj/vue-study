# test

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

# 学んだこと

## スコープ付きCSSのコンパイル方式

htmlのクラス名にユニークなdata属性を付けることでカプセル化を実現している。

## CSSモジュールのコンパイル方式

人間には読めないユニークなクラス名を付けて、そこにcssを当てることでカプセル化を実現している。