<script>
export default {
    data() {
        return {
            menu_2:[
                {
                    option:'DIGITAL COMICS',
                    icon: '/src/assets/images/buy-comics-digital-comics.png'
                },
                {
                    option:'DC MERCHANDISE',
                    icon: '/src/assets/images/buy-comics-merchandise.png'
                },
                {
                    option:'SUBCRIPTION',
                    icon: '/src/assets/images/buy-comics-subscriptions.png'
                },
                {
                    option:'COMIC SHOP LOCATOR',
                    icon: '/src/assets/images/buy-comics-shop-locator.png'
                },
                {
                    option:'DC POWER VISA',
                    icon: '/src/assets/images/buy-dc-power-visa.svg'
                },
            ]
        }
    },
}
</script>
<template lang="">
    <div class="space_black">
    <h6>Content goes here</h6>
    </div>
    <div class="nav_icon">
        <nav>
            <ul>
                <li v-for="(item, index) in menu_2" ::key="index">
                    <a href="#">
                        <img :src="item.icon" :alt="option">
                        {{item.option}}
                    </a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss">
    .space_black{
        width: 100%;
        height: 125px;
        background-color: black;
    }
    h6{
        color: white;
        font-size: 25px;
        padding: 50px;
    }
    .nav_icon{
        padding: 25px;
        width: 100%;
        height: 260px;
        background-color: #0282f9;
    }
    
    ul li {
        padding: 15px;
        color: white;
    }
</style>