# Vue
## Vue引入方法

```html
<script type="module">
import { createApp } from 'https://unpkg.com/vue@3/dist/vue.esm-browser.js';

createApp({
    data() {
        return {
            msg: "hello vue3"
        }
    }
}).mount('#app');
</script>
```

## Vue-bind
```html
 <div id="app">
        <a v-bind:href="url">new web</a>
        <!-- 也可以简化写法 -->
         <a v-bind:href="url">new web</a>
    </div>
    <!-- vue-bind 动态为html标签绑定属性值，如设置href，src，style等 -->
    <script type="module">
            import { createApp, ref } from 'https://unpkg.com/vue@3/dist/vue.esm-browser.js';
                // 创建Vue的app通过creatapp
                createApp({
                    data(){
                        return {
                            url:"https://www.baidu.com"
                        }
                    }

                 }).mount('#app');

    </script>
```
