<template>
 <div class="details">
 <div class="description">
  <span class="label" :style="{backgroundColor: details.videoLabelColor}">{{details.videoLabel}}</span>
  <p class="title">哈哈哈</p>
  <p class="info">
  <i class="iconfont icon--"></i>
  </p>
   <img alt="Vue logo" src="./assets/logo.png">
   <p class="summary">你好靓仔</p>
 </div>
 </div>
</template>
<script>
/* eslint-disable no-undef */
// import axios from 'axios'
// import wx from 'weixin-js-sdk'
export default {
 components: {
 },
 data () {
 return {
  details: {},
  appId: '',
  signature: '',
  timestamp: '',
  nonceStr: '',
  url:''
 }
 },
 beforeDestroy () {
 document.querySelector('.htmlTitle').text = 'title'
 },
 mounted () {
//  axios.get('http://test.murphyyi.com:8080/demo/wechatDemo?appId=wx17db0504203502fd&appSerset=6714e55d259ae02cc8435e580faa849c&url=http%3A%2F%2Ftest.murphyyi.com')
//  .then((res)=>{
//   this.appId = res.data.appId
//   this.signature = res.data.signature
//   this.timestamp = res.data.timestamp
//   this.nonceStr = res.data.nonceStr
//   this.url = res.data.url
//   this.shard()
//   })
//  }
//  ,
//  methods: {
//   shard () {
//     wx.config({
//       debug: true, // 开启调试模式,调用的所有api的返回值会在客户端alert出来，若要查看传入的参数，可以在pc端打开，参数信息会通过log打出，仅在pc端时才会打印。
//       appId: this.appId, // 必填，公众号的唯一标识
//       timestamp: this.timestamp, // 必填，生成签名的时间戳
//       nonceStr: this.nonceStr, // 必填，生成签名的随机串
//       signature: this.signature, // 必填，签名，见附录1
//       jsApiList: ['updateTimelineShareData', 'updateAppMessageShareData']
//     })
//     wx.ready(function () {  
//       wx.updateTimelineShareData({
//           title: "你丑爆了",
//           link: this.url,
//           imgUrl: "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1572024945&di=698f183143b4dd6123faa9b7d0767f46&imgtype=jpg&er=1&src=http%3A%2F%2Fimg1.shikee.com%2Freport%2F2018%2F08%2F17%2F0810450906.jpg", // 分享图标
//           success: function () {
//             alert('分享朋友圈成功')
//           },
//       })
//       wx.updateAppMessageShareData({
//           title: "你好丑",
//           desc: "不！！！你不丑。。。",
//           link: this.url,
//           imgUrl: "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1572024945&di=698f183143b4dd6123faa9b7d0767f46&imgtype=jpg&er=1&src=http%3A%2F%2Fimg1.shikee.com%2Freport%2F2018%2F08%2F17%2F0810450906.jpg", // 分享图标
//           success: function () {
//           alert('分享给朋友成功')
//           },
//         })
//       })
//   }
}
}
</script>
<style lang="less" scoped>
.details {
 overflow: hidden;
 .description {
 padding: 10px;
 .label {
  display: inline-block;
  padding:0 10px;
  height: 22px;
  line-height: 22px;
  color: #fff;
  font-size: 12px;
  text-align: center;
 }
 .title {
  line-height: 30px;
  font-size: 18px;
 }
 .info {
  line-height: 26px;
  color: #949494;
  span {
  margin-right: 15px;
  }
  .iconfont {
  font-size: 12px;
  }
 }
 .summary {
  margin-top: 20px;
  color: #4b4b4b;
  font-size: 16px;
 }
 .article {
  margin-top: 10px;
 }
 }
}
</style>