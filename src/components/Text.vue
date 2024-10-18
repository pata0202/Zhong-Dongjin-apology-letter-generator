<script setup lang="ts">
import { ref } from 'vue'

// defineProps<{ msg: string }>()

const personA = ref('齊廷洹先生');
const personB = ref('齊柏林先生');
const location = ref('苗栗');
const concat = ref('承辦人');
const action = ref('演講')
const personTitle = ref('講者')
const organ = ref('苗栗縣政府')
const organClass = ref('縣')
const manager = ref('科長')

</script>

<template>

    <div class="">
        <h1>鍾東錦道歉信產生器</h1>
        <div class="block">
            <div class="card">
                <span>人物</span>
                <br />
                <input v-model="personA"></input>
                <input v-model="personB"></input>
                <input v-model="action"></input>
                <input v-model="concat"></input>
                <input v-model="personTitle"></input>
                <input v-model="manager"></input>
            </div>
            <div class="card">
                <span>地點</span>
                <br />
                <input v-model="location"></input>
                <input v-model="organ"></input>
                <input v-model="organClass"></input>
            </div>
        </div>
        <p>
            「一定是我做的不夠好，才會養成如此的部屬，{{ personB }}對台灣的貢獻擺在眼前，你怎麼可以如此放肆？」
            <br />
            <br />
            在我所掌理下的{{ organ }}，竟然會有{{ concat }}對前來{{ action }}的{{ personTitle }}說出如此無禮的話？
            是我{{ organ }}的螺絲鬆了，還是我們服務民眾的標準還不夠嚴格？
            看見{{ personA }}臉書上滿滿的委屈，我既痛心又憤怒，他滿懷熱情來到這塊土地，
            而我們留給他的，竟是如此可怕的體驗與屈辱。
            <br />
            <br />
            「這屈辱不但傷害了{{ personA }}，傷害了他的父親，也傷害了整個{{ location }}，我的歉疚與羞慚，難以言喻。」
            {{ concat }}請辭了又如何？{{ manager }}記過又如何？此一事件故鄉所受的傷痕要多少日子才能癒合？
            在我{{ organ }}如果還有如此心態的同仁，請你們立即改正，如若不然，請你離開，我們不容許同樣的錯有第二次發生的可能。
            <br />
            <br />
            「{{ personB }}將台灣推薦給了全世界，而這件不該發生的嚴重錯誤，卻讓{{ location }}辛苦修復的{{ organClass }}譽，關上了燈。」
            <br />
            <br />
            我的世界關了燈，陷入永夜般的黑暗，以致於我翻來覆去，輾轉難眠，因知兵卒欺民皆是將帥無能。
            我不確定{{ personA }}能否接受我的道歉，但{{ personB }}對台灣的貢獻無庸置疑，值此時刻，雖不能聊表歉疚於萬一，但請容我深深一鞠躬，向齊柏林導演致敬。
            「對不起，是我不夠好，讓{{ personA }}與{{ location }}{{ organClass }}民，受了委屈。」
            <br />
            <br />
            {{ organClass }}府同仁們，我們這一路走來不容易，一起善待每個來訪的人，好嗎？
            無論是台灣還是{{ location }}，腳下所踏，都是同一片土地，縱有風雨，我們彼此尊重，唇齒相依。
        </p>
    </div>
</template>

<style scoped>
.block {
    display: block;
    display: flex;
    justify-content: space-between;
}

.card {
    padding: 1em;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 1em;
    width: 50%;
}

input {
    /* display: block; */
    margin-right: 1em;
}
</style>
