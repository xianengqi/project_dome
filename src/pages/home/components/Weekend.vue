<template>
<div>
  <div class="recommend-title">周末去哪儿</div>
  <ul>
    <li class="item border-bottom" v-for="item in recommendList" :key="item.id">
      <div class="item-img-wrapper">   
        <img class="item-img" :src='item.imgUrl'/>
      </div>  
      <div class="item-info">
        <p class="item-title">{{item.title}}</p>
        <p class="item-desc">{{item.desc}}</p>
    
      </div>
    </li>
  </ul>
</div>
</template>
<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
      id: '0001',
      imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3a/f96e254541abb.jpg_r_640x214_6b1fc9f0.jpg',
      title: '鄂西旅游圈',
      desc: '穿越近三千年的历史，仿佛就像昨天'
    },
    {
      id: '0002',
      imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3a/f96e254541abb.jpg_r_640x214_6b1fc9f0.jpg',
      title: '孝感爱琴海水上乐园',
      desc: '穿越近三千年的历史，仿佛就像昨天'
    },
    {
      id: '0003',
      imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3a/f96e254541abb.jpg_r_640x214_6b1fc9f0.jpg',
      title: '孝感爱琴海水上乐园',
      desc: '穿越近三千年的历史，仿佛就像昨天'
    }]
    }
  }
}
</script>
<style lang="stylus" scoped>
@import '~styles/mixins.styl'
  .recommend-title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  .item-img-wrapper
    overflow hidden
    height 0
    padding-bottom 33.9%
    .item-img
      width: 100%
  .item-info
    padding: .1rem    
  .item-title
    line-height .54rem
    font-size .32rem
    ellipsis()
  .item-desc
    line-height .4rem
    color: #ccc
    ellipsis()
    
</style>
