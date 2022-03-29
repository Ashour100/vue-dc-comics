<template>
    <div>
        <div class="top">
            <div class="contentContainer flex">
                <div class="icon flex">
                    <img src="../img/buy-comics-digital-comics.png" alt="">
                    <span>DIGITAL COMICS</span>
                </div>
                <div class="icon flex">
                    <img src="../img/buy-comics-merchandise.png" alt="">
                    <span>DC Merchandise</span>
                </div>
                <div class="icon flex">
                    <img src="../img/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </div>
                <div class="icon flex">
                    <img id="locator" src="../img/buy-comics-shop-locator.png" alt="">
                    <span>COMIC SHOP LOCATOR</span>
                </div>
                <div class="icon flex">
                    <img src="../img/buy-dc-power-visa.svg" alt="">
                    <span>DC POWER VISA</span>
                </div>
            </div>
        </div>
        <div class="middle flex">
            <div class="contentContainer flex">
                <div class="left flex">
                    <div class="list">
                        <h5>DC COMICS</h5>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </div>
                    <div class="list">
                        <h5>DC</h5>
                        <ul>
                            <li>Terms of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certifications</li>
                            <li>Rating</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="list">
                        <h5>SITES</h5>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>Dc Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                    <div class="list shop-list">
                        <h5>SHOP</h5>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                </div>
                <div class="right">
                    <img src="../img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="bottom">
            <div class="contentContainer flex">
                <button>SIGN-UP NOW!</button>
                <div class="socials flex">
                    <h3>FOLLOW US</h3>
                    <img src="../img/footer-facebook.png" alt="">
                    <img src="../img/footer-twitter.png" alt="">
                    <img src="../img/footer-youtube.png" alt="">
                    <img src="../img/footer-pinterest.png" alt="">
                    <img src="../img/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'IndexFooter'
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';
.top{
    height: 18vh;
    background-color: $primary;
    .contentContainer{
        padding: 0 5rem;
    }
    .icon{
        gap: 1rem;
        #locator{
            width: 1.5rem;
        }
        img{
            width: 2.27rem;
        }
        span{
            color: white;
            font-size: .71rem;
        }
    }
    
}
.middle{
    height: 40vh;
    background-image: url('../img/footer-bg.jpg');
    .left{
        color:white;
        flex-wrap: wrap;
        align-items: flex-start;
        width: 20vw;
        text-align: start;
        padding-top: 2rem;
        h5{
            font-weight: 600;
            font-size: .9rem;
        }
        ul{
            padding-left: 0;
            margin-bottom: .1rem;
            font-size: .6rem;
            color:gray;
        }
        li{
            list-style: none;
        }
        .shop-list{
            position: relative;
            bottom:3rem;
        }
    }
    .right{
        // width: 50vw;
        // position: relative;
        // z-index: 1;
        // img{
        //     z-index: 3;
        // }
        display: none;
    }
}
.bottom{
    height:13vh;
    background-color: $secondary;
    button{
        background-color: $secondary;
        color:white;
        border: 2px solid $primary;
        padding: .5rem;
        font-weight: 600;
        font-size: .8rem;
    }
    .socials{
        gap: 1rem;
        img{
            width: 1.8rem;
        }
        h3{
            color: $primary;
            margin: 0;
            font-weight: 700;
            font-size: 1rem;
        }
    }
}
</style>