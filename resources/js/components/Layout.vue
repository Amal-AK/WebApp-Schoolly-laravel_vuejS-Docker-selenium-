<template>
    <body class="h-full flex items-center justify-center bg-green-lightest">
    <div class="bg-blue-darker rounded-lg p-10 m-6">
  <div class="bg-white  flex flex-col " style="font-family: 'Squada One', cursive;  ">
      <div class="container mx-auto px-8">
          <header class="flex flex-col sm:flex-row items-center justify-between px-6 mt-6 relative md:w-full ">
           <div class="flex flex-col sm:flex-row items-center ">
             <router-link to="/Accueil">
                <img alt="logo" src="/images/ghost-green.png" height="100" width="100" >
            </router-link>
                <h3 class="text-4xl font-bold uppercase text-blue-darker  justify-center"> Schoolly</h3>
            </div>
              <nav class="hidden md:flex text-lg">
                   <router-link to="/Accueil" class="text-blue-darker hover:bg-green rounded-lg  py-3 px-6"><i class="fas fa-home"></i> Home</router-link>
                   <router-link to="/Absences" class="text-blue-darker hover:bg-green rounded-lg py-3 px-6"><i class="fas fa-calendar"></i> Absences</router-link>
                   <router-link to="/InscriptionPDG" class="text-blue-darker hover:bg-green rounded-lg py-3 px-6"><i class="fas fa-tools"> </i> Inscription</router-link>
                   <router-link to="/Deconnexion" class="text-blue-darker hover:bg-green rounded-lg py-3 px-6"><i class="fas fa-sign-out-alt"></i> Déconnexion</router-link>
              </nav>
              <button class="flex md:hidden flex-col absolute top-0 right-0 p-4 mt-5">
              </button>
          </header>
          <main class="flex flex-col-reverse sm:flex-row jusitfy-between items-center py-12">
              <div class="sm:w-full flex flex-col items-center sm:items-start text-center sm:text-left">
                
                 <router-view></router-view>

              </div>
          </main>
      </div>
  </div>
</div>
</body>
</template>
<style scoped>
</style>