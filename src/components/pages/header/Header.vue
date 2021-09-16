<template>
    <header class="header">
        <div class="container">
            <div class="header-wrapper">
                <div class="header-brand">
                    <router-link to="/">
                        <img class="logo" src="@/graphics/logo.svg" alt="Электронная приемная граждан Правительства Нижегородской области">
                    </router-link>
                    <div class="header-brand__title">
                        <p class="header-brand__text">Электронная приемная граждан</p>
                        <p class="header-brand__text">Правительства Нижегородской области</p>
                    </div>
                </div>
                <div class="header-controls">
                    <button class="header-controls__btn header-controls__impaired impaired-controls">
                        <p class="impaired-controls__text">
                            Версия для слабовидящих
                        </p>
                        <div class="header-controls__icon"></div>
                    </button>
                    <button class="header-controls__btn header-controls__back back-controls">
                        <a href="#" class="back-controls__link">
                            <p class="back-controls__text">
                                Перейти на портал Правительства
                            </p>
                            <div class="header-controls__icon"></div>
                        </a>
                    </button>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    components: {
    }
}
</script>

<style lang="scss">
.header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: #D9EBF7;
    height: 68px;

    &-wrapper{
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    &-brand{
        display: flex;
        align-items: center;
        &__title{
            margin-left: 10px;
        }
    }
}

.header-controls{
    display: flex;
    position: relative;
    &__btn {
        width: 166px;
        display: flex;
        height: 46px;
        background-color: #E9F5FD;
        border-radius: 6px;
        align-items: center;
        padding: 9px 10px;
    }
    &__btn p {
        font-size: 12px;
        line-height: 14px;
        font-weight: 500;
        text-align: left;
    }
}

.impaired-controls{
    &__text{
        width: 87px;
    }
}

.back-controls{
    margin-left: 30px;
    &__text{
        width: 111px;
    }
}

</style>