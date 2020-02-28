<template>
    <div class="container">
        <div class="progress">
            <div class="title">
                请授权登录....
            </div>
           
            <div class="progressSpot">
                <div class="progresSpotCircular"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
        msg: "Hello",
        URLdata:"asdsad",
        appid:"asas123465498",
        };

    },
    created(){
        console.log("bibibi")
    },
    mounted(){
        // if(this.$route.query.groupid && code == ''  && !this.wxopenid){     //在wxopenid不存在并且微信浏览器内唤起微信授权
        //     spWxGetAppid(this.$route.query.groupid).then(function(res){
        //         var res  = JSON.parse(res.bodyText)
        //         if(res.result=="0"){
        //             window.location.href = "https://open.weixin.qq.com/connect/oauth2/authorize?appid="+res.appid+"&redirect_uri=http://"+this.URLdata+"/oauth.html&response_type=code&scope=snsapi_userinfo&state="+this.$route.query.groupid+"#wechat_redirect"
        //         }else{
        //             this.$vux.alert.show({
        //                 title:"提示",
        //                 content:"获取授权信息失败，请稍后重试"
        //             })
        //         this.clearSession()
        //         }
        //     }.bind(this),function(error){
        //         this.$vux.alert.show({
        //             title:"提示",
        //             content:"获取授权信息失败，请稍后重试"
        //         })
        //         this.clearSession()
        //     })
        // }
    },
    methods: {
        clickHandle() {
            this.msg = "Clicked!!!!!!";
        }
    }
};
</script>

<style>
.container {
  width: 100vmax;
  height: 100vmax;
  background-color: #6170e5;
  display: flex;
  justify-content: center;
  align-items: center;
}
.progress{
    width: 500px;
    height: 500px;
    background-image: url("data:image/png;base64,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");
    background-size: 100% 100%;
    position: absolute;
    top: 20%;
    left: 17%;
    z-index: 10;
    text-align: center;
    color: #ebc697;
}
.progressSpot{
    width: 500px;
    height: 500px;
    animation:lds-hourglass 5.2s infinite;
}
.progresSpotCircular{
    left: 229px;
    top: -5.3px;
    background-color: #f4cd92;
    width: .266667rem;
    height: .266667rem;
    border-radius: 50%;
    position: absolute;
}
@keyframes lds-hourglass {
	0% {
        transform:rotate(-0deg);
    }
    100% {
        transform:rotate(-720deg)
    }
}
.title{
    position: absolute;
    top: 45%;
    left: 33%;
}
</style>