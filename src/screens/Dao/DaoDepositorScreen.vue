<template>
    <v-container fluid>
        <v-row justify="center" class="pa-8">
            <v-col cols="12" md="8">
                <v-card outlined>
                    <v-card-title class="text-h6">
                        Ссылка на внешний интерфейс (iframe) больше не работает
                    </v-card-title>
                    <v-card-text>
                        Мы отключили встраивание по старому URL. Сейчас актуальная информация и
                        функциональность доступны в разделе About.
                    </v-card-text>
                    <v-card-actions>
                        <v-spacer />
                        <v-btn color="primary" @click="$router.push('/about')">
                            Перейти в About
                        </v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
    <!--
    <v-container class="investors" fluid>
        <h1 class="investors__title">For Depositors</h1>
        <div class="investors__content">
            <DaoTable />
        </div>
    </v-container> -->
</template>

<script>
// import DaoTable from '_features/dao/components/DaoTable'

export default {
    name: 'DaoDepositorScreen',
}
</script>

<style lang="scss">
@import "@/sass/_variables.scss";

.investors__title {
    text-align-last: left;
    font-size: $big_font;
    line-height: $big_height;
    font-weight: normal;
    margin-top: 50px;
    margin-bottom: 40px;
    padding-left: 110px;
}
</style>
