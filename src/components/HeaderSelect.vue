<template>
<div id="container">
   <div id="content">
       <button><p>推荐</p> </button>
       <button><p>排行榜</p></button>
       <button><p>歌单</p></button>
       <button><p>主播电台</p></button>
       <button><p>歌手</p></button>
        <button><p>新碟上架</p></button>
   </div>

</div>
</template>
<script>
export default {
    name:'HeaderSelect',
    data() {
        return {
            
        }
    },

}
</script>
<style scoped>
#container{
    width: 100%;
    height:30px;
    background-color: rgb(194,12,12);
}
#content{
    margin: 0 auto;
    width: 900px;
    display:flex;
    justify-content:space-between;
}
button{
    height: 30px;
   background-color: rgb(194,12,12);
   border: none;
   outline: none;
}
button :hover{
background-color: rgb(155,9,9);
border-radius: 3px;
}

</style>