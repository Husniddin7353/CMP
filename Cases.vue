<template>
    <div class="cases">
        <p class="cases__name d-flex align-items-center"> <svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M6 12C9.31371 12 12 9.31371 12 6C12 2.68629 9.31371 0 6 0C2.68629 0 0 2.68629 0 6C0 9.31371 2.68629 12 6 12Z" fill="#F07566"/>
                </svg>  PARTFOLIO
        </p>

        <h1 class="cases__title">
            Company Cases
        </h1>

        <p class="cases__paragraph">
            Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle the same illusion which lifts the horizon of the sea.
        </p>

        <div class="parts">
            <div class="part">
                <img class="part__img" src="@/assets/Bitmap1.png" alt="">
                <a class="part__link" href="#">01</a>

                <h3 class="part__name">
                    Face of Mars
                </h3>

                <p class="part__text">
                    Truly it was a great journey
                </p>
            </div>

            <div class="part">
                <img class="part__img" src="@/assets/Bitmap1.png" alt="">
                <a class="part__link" href="#">02</a>

                <h3 class="part__name">
                    Heavenly Bodies
                </h3>

                <p class="part__text">
                    Truly it was a great journey
                </p>
            </div>

            <div class="part">
                <img class="part__img" src="@/assets/Bitmap1.png" alt="">
                <a class="part__link" href="#">03</a>

                <h3 class="part__name">
                    Liberal Education
                </h3>

                <p class="part__text">
                    Truly it was a great journey
                </p>
            </div>

            <div class="part">
                <img class="part__img" src="@/assets/Bitmap1.png" alt="">
                <a class="part__link" href="#">04</a>

                <h3 class="part__name">
                    Though the Gravity
                </h3>

                <p class="part__text">
                    Truly it was a great journey
                </p>
            </div>

            
        </div>
    </div>
</template>

<script>
export default {
    name:'Cases'
}
</script>

<style lang="scss">

.cases{

    &__name{
        font-weight: bold;
        font-size: 16px;
        line-height: 32px;
        letter-spacing: 1px;
        color: #F07566;
        max-width: 110px;
        margin: 0 auto;

        svg{
            margin-right: 6px;
        }
    }

    &__title{
        font-weight: bold;
        font-size: 56px;
        line-height: 64px;
        text-align: center;
        letter-spacing: -1px;
        color: #333333;
    }

    &__paragraph{
        font-size: 16px;
        line-height: 32px;
        margin: 28px auto 61px auto;
        text-align: center;
        color: rgba(51, 51, 51, 0.496405);
        max-width: 770px;

    }

    .parts{
        display: grid;
        grid-template-columns:1fr 1fr;

        .part{
            border: none;
            position: relative;

            &__link{
                position: absolute;
                bottom: 6.5rem;
                left: 0;
                background: #4DB282;
                border-radius: 0px 24px 0px 8px;
                padding: 20px 20px 20px 30px;
                font-weight: bold;
                font-size: 40px;
                line-height: 48px;
                text-align: center;
                letter-spacing: -1px;
                color: #FFFFFF;
                text-decoration: none;

                &:hover{
                    background-color: #98e4bf;
                    color: #4DB282;
                    transition: all 0.3s ;
                }
            }

            &__name{
                font-weight: bold;
                font-size: 24px;
                line-height: 32px;
                text-align: center;
                color: #333333;
                padding: 8px 0;
            }

            &__text{
                font-size: 16px;
                line-height: 32px;
                text-align: center;
                color: rgba(51, 51, 51, 0.496405);
            }
        }
    }
}

@media  screen and (max-width:980px){
    .parts{
        display: flex !important;
        flex-direction: column;

        .part{
            &__img{
                max-width: 80%;
                margin-left: 10%;
            }
            &__link{
                margin-left: 10%;
            }
        }
    
    }
}

</style>