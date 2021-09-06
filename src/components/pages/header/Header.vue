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
                    <button class="header-controls__back back-controls">
                        <a href="#" class="back-controls__link">
                            <p class="back-controls__text">
                                Перейти на портал Правительства
                            </p>
                            <div class="back-controls__arrow"></div>
                        </a>
                    </button>
                </div>
            </div>

        </div>
    </header>
</template>

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
    }
}

</style>

<script>
export default {
    components: {
    }
}
</script>