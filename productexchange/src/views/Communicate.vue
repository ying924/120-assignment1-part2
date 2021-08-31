<template>
  <div>
    <h1>Apple MacBook Air</h1>
    <div class="talk_con">
        <div class="talk_show" id="words">
            <div class="atalk"><span id="asay">Robert：how about this？</span></div>
            <div class="btalk"><span id="bsay">me：Yes, I want to buy</span></div>
        </div>
        <div class="talk_input">
            <input type="button" class="imageBtn" value="image">
            <input type="text" class="talk_word" id="talkwords">
            <input type="button" value="send" class="talk_sub" id="talksub">
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
h1{
     text-align: center;
}
.talk_con{
    width:600px;
    height:500px;
    border:1px solid #666;
    margin:50px auto;
    background:#f9f9f9;
}
.talk_show{
    width:99%;
    height:420px;
    border:1px solid #666;
    background:#fff;
    margin:10px auto;
    overflow:auto;
}
.talk_input{
    width:580px;
    margin:0 auto;
}
.imageBtn{
    width:80px;
    height:30px;
    float:left;
    outline:none;
}
.talk_word{
    width:420px;
    height:26px;
    padding:0px;
    float:left;
    outline:none;
    text-indent:10px;
}        
.talk_sub{
    width:56px;
    height:30px;
    float:left;
}
.atalk{
  margin: 10px auto auto -350px; 
}
.atalk span{
    background:#0181cc;
    border-radius:10px;
    color:#fff;
    padding:5px 10px;
    margin-left: -10px;
}
.btalk{
    margin:10px;
    text-align:right;
}
.btalk span{
    background:#ef8201;
    border-radius:10px;
    color:#fff;
    padding:5px 10px;
}
</style>