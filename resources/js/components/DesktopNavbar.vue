<template>
	<section id="desktop-nav">
		<nav class="navbar-light bg-light shadow py-2">
			<div
				class="
					container-fluid
					d-flex
					justify-content-around
					align-items-center
					py-2
				"
			>
				<div class="d-flex align-items-center">
					<img
						id="logo"
						:src="'./img/pubb/deliveboo_loader.gif'"
						class="img-fluid"
						alt="Logo Deliveboo"
					/>
					<div class="h1 m-0 pl-3 t-deliveboo-green fw-bold koulen">
						DELIVEBOO
					</div>
				</div>
				<div class="d-flex justify-content-between align-items-center">
					<div>
						<router-link to="/" class="text-decoration-none router-link">
							<i class="fas fa-home t-deliveboo-green"></i>
							<span class="text nav-text t-deliveboo-green ml-1 koulen"
								>Home</span
							>
						</router-link>

						<router-link to="/restaurants" class="text-decoration-none">
							<i class="fas fa-utensils t-deliveboo-green"></i>
							<span class="text nav-text t-deliveboo-green ml-2 koulen"
								>Ristoranti</span
							>
						</router-link>
					</div>

					<div>
						<a href="/admin" class="text-decoration-none">
							<i class="fas fa-user t-deliveboo-green"></i>
							<span class="text nav-text t-deliveboo-green ml-2 koulen"
								>Login</span
							></a
						>
						<a href="/register" class="text-decoration-none">
							<i class="far fa-user t-deliveboo-green"></i>
							<span class="text nav-text t-deliveboo-green ml-2 koulen"
								>Register</span
							></a
						>
					</div>
				</div>
			</div>
		</nav>
	</section>
</template>

<script>
export default {
	name: "DesktopNavbar",
};
</script>

<style lang="scss" scoped>
a.active span {
	color: #007377;
	font-size: 20px;
}

a.active i {
	font-size: 1.5em;
	color: #007377;
}

#logo {
	max-width: 60px;
}

i {
	margin-left: 40px;
	font-size: 18px;
}

a {
	text-decoration: none;
}

.koulen {
	font-family: "Koulen", cursive;
}
</style>