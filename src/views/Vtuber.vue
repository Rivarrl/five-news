<template>
    <div id="vtuber">
        <div id="citiao">
            <div>
                <button>ALL</button>
                <button>6⭐</button>
                <button>5⭐</button>
                <button>4⭐</button>
                <button>3⭐</button>
                <button>2⭐</button>
                <button>1⭐</button>
            </div>
            <div>
                <p>资质</p>
                <button>新手</button>
                <button>资深干员</button>
                <button>高级资深干员</button>
            </div>
            <div>
                <p>位置</p>
                <button>远程位</button>
                <button>近战位</button>
            </div>
            <div>
                <p>种类</p>
                <button>先锋干员</button>
                <button>狙击干员</button>
                <button>医疗干员</button>
                <button>术师干员</button>
                <button>近卫干员</button>
                <button>重装干员</button>
                <button>辅助干员</button>
                <button>特种干员</button>
            </div>
            <div>
                <p>词缀</p>
                <button>治疗</button>
                <button>支援</button>
                <button>输出</button>
                <button>群攻</button>
                <button>减速</button>
                <button>生存</button>
                <button>防护</button>
                <button>削弱</button>
                <button>位移</button>
                <button>控场</button>
                <button>爆发</button>
                <button>召唤</button>
                <button>快速复活</button>
                <button>费用回复</button>
                <button>支援机械</button>
            </div>
            <div>
                <button>清空</button>
                <button>屏蔽三星以下干员</button>
            </div>
        </div>
        <div id="juese">角色</div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="stylus">
#citiao 
    width 40%
    height 90vh
    float left 
    overflow hidden
    user-select none
    background #16181c
    color #000000
#juese
    width 40%
    height 90vh
    overflow hidden
    user-select none
    background #ffffff
    color #000000
button  
    background  #000000
    text-align middle 
    color #ffffff
    border-radius 20px 
    margin 5px
p
    color #ffffff    
</style>