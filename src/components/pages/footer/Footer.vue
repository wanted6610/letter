<template>
    <footer class="footer">
        <div class="container">
            <div class="information">
                <div class="information-copy">
                    <p class="information-copy__copyright">
                        {{information.copyright}}
                    </p>
                    <p class="information-copy__title">
                        {{information.title}}
                    </p>
                </div>
                <div class="information-contacts">
                    <p class="information-contacts__adress">
                        {{information.adress}}
                    </p>
                    <p class="information-contacts__phone">
                        {{information.phone}}
                    </p>
                    <p class="information-contacts__mail">
                        {{information.mail}}
                    </p>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    data() {
        return {
            information: {
                copyright: '© 2020 Правительство Нижегородской области, официальный портал',
                title: 'Электронная приемная граждан',
                adress: '603134, г. Нижний Новгород, ул. Костина, д. 2, 1 этаж, каб. 22',
                phone: 'Телефон приемной: +7 (831) 439-04-98',
                mail: 'E-mail: priem@org.kreml.nnov.ru',
            }
        }
    }
}
</script>

<style scoped lang="scss">
.footer {
    height: 154px;
    background-color: #273E4E;
    display: flex;
    align-items: center;
}

.information {
    display: flex;
    align-items: center;
    justify-content: space-between;
    
    p {
        margin: 12px 0;
        color: #fff;
    }

    &-copy {
        text-align: left;
    }

    &-contacts {
        text-align: right;
    }
}
</style>