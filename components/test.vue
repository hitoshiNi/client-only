<template>
    <div>
      <button v-on:click="openModel">利用規約を確認</button>
      <button class="button" v-bind:disabled="!apply">ツイートして応募</button>
      <div v-show="showContent">
         <form>
         <input type="checkbox" v-model="agree">利用規約に同意する<br>
         <input type="checkbox" v-model="follow">キャンペーンアカウントをフォローする<br>
         </form>
        <button v-on:click="closeModel" class="button">ページを閉じる</button>
      </div>
    </div>

</template>

<script>
export default {
    data(){
        return{
            showContent:false,
            agree:false,
            follow:false,
            apply:false,
        }
    },
    methods:{
        openModel:function(){
            this.showContent=true;
            console.log(this.showContent);
            console.log(this.agree);
            console.log(this.follow);
            console.log(this.apply);
        },
        closeModel:function(){
            this.showContent=false;
            this.apply=this.agree&&this.follow;
        }
    }
}
</script>