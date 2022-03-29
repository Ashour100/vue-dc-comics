<template>
    <div class="header">
            <div class="header-logo">
                <img src="../img/dc-logo.png" alt="">
            </div>
            <div class="header-nav">
                <ul>
                    <li v-for="(link, index) in headerLinks" :key="index"  :class="(link.current==true)?'active':''" >
                        <a :href="link.url" @click="setActivePage(index)">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </div>
    </div>
</template>

<script>
export default {
    name:'IndexHeader',
    data: function() {
        return {
            headerLinks:[
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ],
        }
    },
    methods:{
        setActivePage(index){
            this.headerLinks.forEach(element => {
                element.current=false;
            });
            this.headerLinks[index].current=true;
        }
    }
}
</script>

<style lang="scss" scoped>
.header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 10rem;
    height: 15vh;
}
.header-logo{
    img{
        width: 85%;
    }
}
.header-nav{
    height: 100%;
    ul{
        height: 100%;
        margin: 0;
        display: flex;
        li{
            list-style: none;
            padding: 0 .7rem;
            height: 100%;
            display: flex;
            align-items:center;
            a{
                text-decoration: none;
                color: black;
                vertical-align: 1rem;
            }
        }
    }
}
.active{
    border-bottom: 5px solid rgb(42, 42, 255);
    a{
        color: rgb(42, 42, 255) !important;
    }
    
}

</style>