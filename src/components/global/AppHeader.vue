<template>
    <div class="header">
        <div class="container">
            <div class="logo">
                <router-link to="/" exact>
                    <a>Crescent</a>
                </router-link> 
            </div>
            <ul class="text-end ">
                <router-link to="/" tag="li" exact>
                <a>Home</a> 
                </router-link> 
                <router-link to="/about"  tag="li">
                <a>About</a>
                </router-link>  
                <router-link to="/Blog"  tag="li">
                <a>Blog</a>
                </router-link>
                <router-link to="/helpe"  tag="li">
                <a>Helpe</a>
                </router-link>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    name:'AppHeader'
}
</script>

<style lang="scss" scoped>
.header{
    background-color: #333;
    color: #fff;
    overflow: hidden;
    .logo{
        font-size: 24px;
        padding: 20px;
        float: left;
        width: 200px;
         a{
                color: #fff;
                text-decoration: none;
            }
    }
    ul{
        float: left;
        width: calc(100% - 200px);
        margin: 0;
        li{
            padding: 20px;
            display: inline-block;
            font-size: 18px;
            a{
                color: #fff;
                text-decoration: none;
            }
        }
    }
}
</style>