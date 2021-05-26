<template>
<div class="parent">
    <h2>{{ msg }}</h2>
    <son psMsg="父传子的内容:叫爸爸"></son> <!-- 子组件绑定psMsg变量-->
</div>
</template>
<script>
import son from './Son'//引入子组件
export default {
    name: 'HelloWorld',
    data(){
        return {
            msg: '父组件'
        }
    },
    components: {
        son
    }
}
</script>
