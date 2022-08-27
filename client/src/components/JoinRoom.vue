<script setup>
	
</script>

<template>
	<div class="joinRoom" id="joinRoom">
		<div class="header">
			<h2>Join Room</h2>
		</div>
		<form class="joinRoomForm">
			<div class="form-control">
				<label for="username">Username</label>
				<input type="text" name="username" id="username-field" placeholder="Type your Username">
			</div>
			<div class="form-control">
				<label for="room-number">Room</label>
				<input type="text" name="room-number" id="room-number" placeholder="Type Room Number">
			</div>
			<button class="roomJoinBtn" @click.prevent="">JOIN</button>
		</form>
	</div>
</template>

<style scoped lang="scss">
	.joinRoom{
		width: 600px;
		height: auto;
		background: $secondary-black;
		border-radius: 10px;
		padding:20px;
		.header{
			position: relative;
			margin-bottom: 50px;
			h2{
				font-size: 30px;
				font-weight: bolder;
			}
		}
		.joinRoomForm{
			width: 100%;
			height: auto;
			.form-control{
				width: 100%;
				margin-bottom: 20px;
				label{
					display: block;
					margin-bottom: 10px;
				}
				input{
					width: 100%;
					height: 40px;
					border-radius: 5px;
					outline: none;
					border: none;
					background:$primary-black;
					padding: 10px;
				}
				&:nth-child(2){
					margin-bottom: 30px;
				}

			}


			.roomJoinBtn{
				width: 100%;
				height: 40px;
				font-size: 20px;
				background: $primary-red;
				border: none;
				outline: none;
				cursor: pointer;
				border-radius: 5px;
				font-weight: 600;
			}
		}
	}
</style>