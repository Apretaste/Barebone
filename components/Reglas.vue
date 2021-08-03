<template>
	<div>
		<!-- title -->
		<ap-title :data="title"></ap-title>

		<!-- text -->
		<ap-text class="mb-3" :data="text"></ap-text>

		<!-- rules -->
		<ap-rules :data="rules"></ap-rules>

		<!-- floating action button -->
		<ap-fab :data="fab"></ap-fab>
	</div>
</template>

<script>
	module.exports = {
		data: function () {
			return {
				title: {text: 'Reglas'},
				text: {text: 'Este es un ejemplo de lista de reglas para usar en los servicios que requieran ayuda.'},
				rules: [
					{title:'Esto es lo primero que debes saber', text:'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor salvi@apretaste.org incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.'},
					{title:'Esto es lo segubndo mas importante que debes saber', text:'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.'},
					{text:'Lorem ipsum dolor sit amet, consectetur a @salvipascual adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.'},
					{title:'Y aca, viene la bomba', text:'Lorem ipsum dolor sit amet, https://www.apretaste.org consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.'},
				],
				fab: [
					{icon:'fas fa-arrow-left', onTap:function(){ apretaste.back() }}
				]
			}
		}
	}
</script>

<style scoped>
</style>
