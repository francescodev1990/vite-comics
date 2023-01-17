<script>
export default {
    data() {
        return {
            menu: [
                {
                    label: 'Personaggi',
                    url: '#',
                    active: false
                },
                {
                    label: 'Cartoni',
                    url: '#',
                    active: false
                },
                {
                    label: 'Film',
                    url: '#',
                    active: false
                },
                {
                    label: 'TV',
                    url: '#',
                    active: false
                },
                {
                    label: 'Giochi',
                    url: '#',
                    active: false
                },
                {
                    label: 'Collezionabili',
                    url: '#',
                    active: false
                },
                {
                    label: 'Video',
                    url: '#',
                    active: false
                },
                {
                    label: 'Fans',
                    url: '#',
                    active: false
                },
                {
                    label: 'News',
                    url: '#',
                    active: false
                },
                {
                    label: 'Shop',
                    url: '#',
                    active: false
                },
            ]
        }
    },
    
}
</script>
<template lang="">
    <header>
        <a href="/" class="brand">
            <img src="../assets/images/dc-logo.png">
        </a>
        <nav>
            <ul>
                <li v-for="item in menu">
                    <a :href="item.url" :class="item.active ? 'active' :''"></a>

                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss">
    header{
        text-align: center;
        margin-top: 25px;
    }
</style>