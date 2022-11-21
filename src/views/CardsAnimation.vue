<template>
	<div class="flex-container">
		<div style="flex-grow: 1">1 1/3</div>
		<div style="flex-grow: 1">2 1/3</div>
		<div style="flex-grow: 1">3 1/3</div>
	</div>
	<div class="flex-container">
		<div style="flex-grow: 1">
			<div class="card">
				<img src="../assets/logo.png" alt="logo" />
				<div class="container">
					<h4>hey mom</h4>
					<p>living la vie da loca</p>
				</div>
			</div>
		</div>
		<div style="flex-grow: 1">
			<div class="card">
				<img src="../assets/logo.png" alt="logo" />
				<div class="container">
					<h4>hey mom</h4>
					<p>living la vie da loca</p>
				</div>
			</div>
		</div>
		<div style="flex-grow: 1">
			<div class="card">
				<img src="../assets/logo.png" alt="logo" />
				<div class="container">
					<h4>hey mom</h4>
					<p>living la vie da loca</p>
				</div>
			</div>
		</div>
	</div>

	<div class="row">
		<div class="col-m-4">
			<div class="card">
				<img src="../assets/logo.png" alt="logo" />
				<div class="container">
					<h4>hey mom</h4>
					<q>
						Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quisquam nihil
						non molestias fuga hic quos commodi quod veritatis? Vel velit laudantium
						perferendis repudiandae quod ducimus aut dolorum fugiat consequatur
						necessitatibus.
					</q>
					<p>living la vie da loca</p>
				</div>
			</div>
		</div>
		<div class="col-m-4">
			<div class="card">
				<img src="../assets/logo.png" alt="logo" />
				<div class="container">
					<h4>hey mom</h4>
					<q>
						Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quisquam nihil
						non molestias fuga hic quos commodi quod veritatis? Vel velit laudantium
						perferendis repudiandae quod ducimus aut dolorum fugiat consequatur
						necessitatibus.
					</q>
					<p>living la vie da loca</p>
				</div>
			</div>
		</div>
		<div class="col-m-4">
			<div class="card">
				<img src="../assets/logo.png" alt="logo" />
				<div class="container">
					<h4>hey mom</h4>
					<q>
						Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quisquam nihil
						non molestias fuga hic quos commodi quod veritatis? Vel velit laudantium
						perferendis repudiandae quod ducimus aut dolorum fugiat consequatur
						necessitatibus.
					</q>
					<p>living la vie da loca</p>
				</div>
			</div>
		</div>
	</div>
</template>
<script lang="ts"></script>
<style lang="scss" scoped>
.card {
	box-shadow: 0 4px 8px 0 rgba($color: #000000, $alpha: 0.2);
	transition: 0.5s;
	background: #fba92c;
	color: #000000;
	cursor: pointer;
	border-radius: 10px;
	padding: 10px;
	&:hover {
		box-shadow: 0 8px 16px 0 rgba($color: #000000, $alpha: 1);
		background: #ffffff;
	}
	display: grid;
	grid-template-rows: repeat(2, 1fr);
	img {
		place-self: center;
	}
	.container {
		text-align: left;
		padding: 10px;
	}
}
</style>
