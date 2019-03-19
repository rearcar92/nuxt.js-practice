<template>
    <header>
        <div id="logo">
            <figure>
                <img src="~/assets/image/test_logo.png" alt="">
            </figure>
        </div>
        <nav id="nav_flex">
            <router-link 
                v-for="routes in links" 
                v-bind:key="routes.id"
                :to="`${routes.page}`">
                {{routes.text}}
            </router-link>
        </nav>            
    </header>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          id: 0,
          text: '메인',
          page:'/mainHeader'
        },
        {
          id: 1,
          text: '풀터',
          page:'/mainFooter'
        },
        {
          id: 2,
          text: 'index',
          page:'/'
        }
      ]
    }
  }
}
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
    }
    #logo {
        width: 50px;
        box-sizing: border-box;
        justify-content: flex-start;
        padding: 5px;
        margin: 0 0 0 20px;
    }
    #logo figure img {
        max-width: 100%;
    }
    #nav_flex {
        display: flex;
        justify-content: flex-end;
        margin: 0 20px 0 0;
    }
    #nav_flex > a {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 0 10px;
        font-size: .8rem;
        text-decoration: none;
    }
    #nav_flex > a:visited {
        color: #000;
    }
</style>
