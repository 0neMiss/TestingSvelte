<script>
	export let  firstName = 'Jordan';
	export let lastName = 'Shehane';
	export let color = 'blue'
	export let showText = true
	export let users = [
		{
			id: 1,
			name: 'Ellie'
		},
		{
			id: 2,
			name: 'Wen Wen'
		},
		{
			id: 3,
			name: 'Jordan'
		},

	]
	$: name = firstName + ' ' + lastName 
	const togggle = ()=>{
		color = color === 'blue' ? 'red' : 'blue'	
		showText = !showText
		users = [...users, {}]
	}
</script>

<main>
	<h1>Hello {name}!</h1>
</main>

<style>


	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>