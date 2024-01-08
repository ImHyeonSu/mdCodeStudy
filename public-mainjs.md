2024.01.06
=============
# main.js

・npm run serveコマンドを実行した時に最初実行されるファイル、vueのインスタンスを作られる
・main.jsに宣言してた全域ファイルは他のvueなどでも使える

```javascript
import commonJs from '@/assets/js/common';
import constJs from '@/assets/js/const';

Vue.use(commonJs);
Vue.use(constJs);
Vue.prototype.$global = {

    // ログインユーザー情報
    loginUser: null,
}
// vueインスタンス作成
// windowの要素にvueInsというvueインスタンスを追加する
window.vueIns = new Vue({
    // vuetifyというVue.jsのUIframework使用
    vuetify,
    // Vue Routerを使用するための設定
    router,
    // Appというコンポーネントをrender、
    render: h => h(App)
    // indexl.htmlの id = appと言うところに連結される
}).$mount('#app')
```