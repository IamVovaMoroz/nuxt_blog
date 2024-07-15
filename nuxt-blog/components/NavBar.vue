<template>
	<div>
	  <nav class="navbar">
		<ul class="navbar-nav">
		  <li class="nav-item"><NuxtLink to="/">Home</NuxtLink></li>
		  <li class="nav-item"><NuxtLink to="/about">About</NuxtLink></li>
		  <li class="nav-item"><NuxtLink to="/services">Services</NuxtLink></li>
		  <li class="nav-item"><NuxtLink to="/pricing">Pricing</NuxtLink></li>
		  <li class="nav-item"><NuxtLink to="/contact">Contact</NuxtLink></li>
		</ul>
	  </nav>
	</div>
  </template>
  
  <script>
  export default {
  
  }
  </script>
  
  <style lang="scss" scoped>
  .navbar {
	background-color: #fff; /* белый фон для навбара */
	padding: 1rem; /* отступы внутри навбара */
	.navbar-nav {
	  list-style-type: none; /* убрать маркеры списка */
	  padding: 0;
	  margin: 0;
	  display: flex; /* выстроить элементы в одну линию */
	  justify-content: space-around; /* равномерное распределение элементов */
	  .nav-item {
		a {
		  text-decoration: none; /* убрать стандартное подчеркивание ссылок */
		  color: #000; /* черный цвет текста */
		  padding: 0.5rem 1rem; /* отступы у ссылок */
		  transition: all 0.3s ease; /* плавный переход для эффекта при наведении */
		  &:hover {
			border-bottom: 2px solid #000; /* нижнее подчеркивание при наведении */
		  }
		}
	  }
	}
  }
  </style>
  