<template>
    <div class="app">
        <Header class="header">

        </Header>  
        <div class="main">
            <Nuxt />
        </div>
        <Footer class="footer">

        </Footer>
    </div>
</template>
<script>
export default {
}
</script>

<style lang="scss" scoped>
.app{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-rows: 2rem 1fr 2rem;
    height: 100vh;
    grid-template-areas: 
        "header header header header"
        "main main main main"
        "footer footer footer footer";
}

.header{
    grid-area: header;
}

.main{
    grid-area: main;
}

.footer{
    grid-area: footer;
}
</style>

