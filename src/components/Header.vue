<template>
	<div class="header-container">
	  <div class="header">
	  	<div class="container">
	  		<!-- <div>Ícones feitos por <a href="https://www.flaticon.com/br/autores/freepik" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/br/" title="Flaticon">www.flaticon.com</a></div> -->
	  		<div class="button-navigations">
	  			<div class="menu-bars" @click="menuLateralAtivo = !menuLateralAtivo">
	  				<i class="fas fa-bars" style="width: 36px;"></i>
	  			</div>

	  			<div class="menu-logo">
	  				<a href="/"><img src="../assets/youtube-logo.png"></a>
	  			</div>
	  		</div>
  		
  			<form id="search-form" class="search-form">  				
	  			<input type="text" name="search">
	  			<button type="submit"><i class="fas fa-search"></i></button>
  			</form>

	  		<div class="icons-perfil">
	  			<ul>
	  				<li><a href="#"><i class="fas fa-video"></i></a></li>
	  				<li><a href="#"><i class="fas fa-grip-vertical"></i></a></li>
	  				<li><a href="#"><i class="fas fa-bell"></i></a></li>
	  				<li><a href="#">
	  					<img class="profile-image" src="../assets/channel.jpg" alt="">
	  				</a></li>
	  			</ul>
	  		</div>
	  	</div>
	  </div>

	  <transition name="fade">
	  	<SideBarMenu v-show="menuLateralAtivo" />
		</transition>
	</div>
</template>

<script>

import SideBarMenu from "./SideBarMenu"

export default {
  name: 'Header',
  data: () => {
  	return {
  		menuLateralAtivo: true
  	}
  },
  components: {
  	SideBarMenu
  }
}
</script>
<style scoped>
	.header-container {
		width: 100%;
		height: 56px;
	}

	.header {
		width: 100%;
		height: 56px;
		background: #fff;
		display: flex;
		align-items: center;
	}

	.container {
		width: 100%;
		display: flex;
		margin: 0px 20px;
		align-items: center;
		justify-content: space-between;
	}

	.button-navigations {
		display: flex;
		align-items: center;
	}

	.menu-logo {
		width: 85px;
		margin: 0px 20px;
	}

	.fade-enter-active,
	.fade-leave-active {
	  transform: translate3d(0, 0, 0);
	  transition: .3s;
	}

	.fade-enter,
	.fade-leave-to {
	  transform: translate3d(-300px, 0, 0);
	}


	.search-form {
		width: 40%;
		height: 30px;
		border: 1px solid #E5E5E5;
		display: flex;
	}

	.search-form input {
		width: 90%;
		padding: 5px 15px;
		outline: 0;
		border: none;
	}

	.search-form button {
		padding: 5px 25px;
		background: #F0F0F0;
		color: #606060;
		cursor: pointer;
		border-right: 1px solid #E5E5E5;
		border:none;
	}

	.search-form button:hover {
		color: #333;
	}

	.search-form input:focus {
		border-color: none;
	}

	.icons-perfil ul {
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.icons-perfil ul li {
		width: 32px;
		height: 32px;
		margin-top: 15px;
		margin-left: 15px;
	}

	.icons-perfil ul li a {
		color: #333;
	}

	.icons-perfil ul li:last-child {
		margin-top: 0px;
	}

	.profile-image {
		width: 32px;
		height: 32px;
		border-radius: 50%;
	}
</style>