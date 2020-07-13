<template>
	<div class="sidebar">
		<ul class="sidebar-roads">
			<li>
				<a href="#">
					<span><i class="fas fa-home"></i></span>
					<p>Início</p>
				</a>
			</li>
			<li>
				<a href="#">
					<span><i class="fas fa-fire"></i></span>
					<p>Em alta</p>
				</a>
			</li>
			<li>
				<a href="#">
					<span><i class="fas fa-folder-open"></i></span>
					<p>Inscrições</p>
				</a>
			</li>
		</ul>
		<ul class="sidebar-roads">
			<li>
				<a href="#">
					<span><i class="fas fa-book"></i></span>
					<p>Biblioteca</p>
				</a>
			</li>
			<li>
				<a href="#">
					<span><i class="fas fa-history"></i></span>
					<p>Histórico</p>
				</a>
			</li>
			<li>
				<a href="#">
					<span><i class="fas fa-clock"></i></span>
					<p>Assistir mais tarde</p>
				</a>
			</li>
			<li>
				<a href="#">
					<span><i class="fas fa-thumbs-up"></i></span>
					<p>Videos marcados co...</p>
				</a>
			</li>
			<li>
				<a href="#">
					<span><i class="fas fa-list"></i></span>
					<p>Playlist</p>
				</a>
			</li>
		</ul>
		<ul class="sidebar-subscriptions">
			<h3>Inscrições</h3>
			<li>
				<a href="#">
					<img src="../assets/channel.jpg">
					<p>Douglas Nicolas</p>
				</a>
			</li>
			<li>
				<a href="#">
					<img src="../assets/channel.jpg">
					<p>Douglas Nicolas</p>
				</a>
			</li>
			<li>
				<a href="#">
					<img src="../assets/channel.jpg">
					<p>Douglas Nicolas</p>
				</a>
			</li>
		</ul>
	</div>
</template>

<script>
	export default {
		name: 'SideBarMenu'
	}
</script>

<style scoped>
	.sidebar {
		width: 240px;
		height: 110vh;
		background: #fff;
	}

	.sidebar ul {
		border-bottom: 1px solid #E5E5E5;
		padding: 10px 0px;
	}

	.sidebar .sidebar-roads li a {
		display: flex;
		color: #606060;
		padding: 12px 30px;
	}

	.sidebar .sidebar-roads li a:hover {
		background: #E5E5E5;
	}

	.sidebar .sidebar-roads li a span {
		width: 18px;
	}

	.sidebar .sidebar-roads li a p {
		margin-left: 15px;
		font-size: 14px;
		line-height: 21px;
		color: #030303;
	}

	.sidebar .sidebar-subscriptions {
		display: flex;
		flex-direction: column;
		margin: 0 15px;
	}

	.sidebar .sidebar-subscriptions h3 {
		color: #626262;
		margin: 10px 0px;
		font-size: 14px;
		text-transform: uppercase;
	}

	.sidebar .sidebar-subscriptions li a {
		display: flex;
		margin: 5px 0px;
		align-items: center;
	}

	.sidebar .sidebar-subscriptions li a img {
		width: 32px;
		height: 32px;
		border-radius: 50%;
	}

	.sidebar .sidebar-subscriptions li a p {
		margin-left: 15px;
		font-size: 14px;
		line-height: 21px;
		color: #030303;
	}
</style>