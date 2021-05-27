<template>
  <div>
    <b-button class="menu" v-b-toggle.sidebar-variant><b-icon-plus-square></b-icon-plus-square></b-button>
    <b-sidebar id="sidebar-variant" title="" bg-variant="dark" text-variant="light" no-header right shadow sidebar-class="border-left border-danger">        
    <template #default="{ hide }">
      <div class="px-3 py-2 margin">          
        <!--<p>
          "Las complicaciones surgen, se consideran y se superan"
        </p>-->
        <img class="img-fluid img-profile rounded-circle mx-auto mb-2" src="../assets/leonel.png" alt="">
        <nav class="mb-3 sidebar-nav left">
            <b-nav vertical>
              <b-nav-item class="sidebar-brand" active @click="hide" v-b-modal="'acercademi'"><b-icon-person-lines-fill></b-icon-person-lines-fill> Acerca de mi</b-nav-item>
              <b-nav-item class="sidebar-brand" @click="hide" v-b-modal="'experiencia'"><b-icon-code></b-icon-code> Experiencia</b-nav-item>
              <b-nav-item class="sidebar-brand" @click="hide" v-b-modal="'educacion'"><b-icon-building></b-icon-building> Educación</b-nav-item>
              <b-nav-item class="sidebar-brand" @click="hide" v-b-modal="'skills'"><b-icon-cpu></b-icon-cpu> Skills</b-nav-item>
              <b-nav-item class="sidebar-brand" @click="hide" v-b-modal="'portafolio'"><b-icon-cloud-arrow-up></b-icon-cloud-arrow-up> Portafolio</b-nav-item>
            </b-nav>
          </nav>         
          <b-button class="menu" block @click="hide"><b-icon-file-minus></b-icon-file-minus></b-button>               
      </div>      
      </template>
    </b-sidebar>
  </div>
</template>
<style scoped>
.menu{
    position: fixed;
    right: 15px;
    top: 15px;
    width: 60px;
    height: 65px;
    text-align: center;
    color: #fff;
    background: rgba(52,58,64,.7);
    line-height: 50px;
    z-index: 999;
}
.margin{
    margin-top: 25%;
}
.sidebar-nav {
    list-style: none;
}

.img-profile {
    max-width: 10rem;
    max-height: 10rem;
    border: 0.5rem solid rgba(255, 255, 255, 0.2);
}

.sidebar-nav > .sidebar-brand {
    font-size: 1.2rem;
    background: rgba(52,58,64,.1);
    height: 80px;
    line-height: 50px;
    padding-top: 15px;
    padding-bottom: 15px;
    padding-left: 15px;
}

</style>