<template>
    <navbar position="fixed"
            type="white"
            menu-classes="ml-auto">

        <template slot-scope="{toggle, isToggled}">
            <router-link v-popover:popover1 class="" to="/accueil">
                <div class="logo-img" style=""> </div>
            </router-link>
        </template>


        <template slot="navbar-menu">
            <router-link class="nav-item nav-link" to="/accueil">
                Accueil
            </router-link>

            <router-link class="nav-item nav-link" to="/particulier">
                Particulier
            </router-link>

            <router-link class="nav-item nav-link" to="/presentation">
                Entreprise
            </router-link>

            <router-link class="nav-item nav-link" to="/presentation">
                Conditions générales
            </router-link>

            <router-link class="nav-item nav-link" to="/contact">
                Contact
            </router-link>

        </template>
    </navbar>
</template>

<script>
  import { DropDown, NavbarToggleButton, Navbar, NavLink } from '@/components';
  import { Popover } from 'element-ui'

  export default {
    name: 'main-navbar',
    components: {
      DropDown,
      Navbar,
      NavbarToggleButton,
      NavLink,
      [Popover.name]: Popover
    }
  }
</script>

<style scoped>
    .logo-img{
        background-image: url('/img/icons/logo-horizont.jpg');
        background-size: contain;
        background-repeat: no-repeat;
        height:60px;
        width:200px;
        display: inline-block;
    }
    .navbar-brand {
        padding-top: 0 ;
        padding-bottom: 0;
    }

</style>
