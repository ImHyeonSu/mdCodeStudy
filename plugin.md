2024.01.06
=============
# plugin

## plugin作成
```javascript
// この二つの書き方でpluginファイルを作成
export default {
    install: (app,options) =>{

    }
}
or

export default {
    install(Vue){

    }
}
```
## 説明
外部ライブラリを使用したり、追加的な機能を拡張するために全域レベルの機能をVueに追加することをPluginという
