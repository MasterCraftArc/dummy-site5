<script>
	import Card from './Card.svelte';
	import CardGlow from '../Home/CardGlow.svelte';
	import yellowGlow from '../../images/svg/yellow-glow.svg';
	import blueGlow from '../../images/svg/blue-glow.svg';
</script>

<section class="section4">
	<div class="card-glow"><CardGlow glowLeft={yellowGlow} glowRight={blueGlow} /></div>
	<Card
		title="Rapid ATO"
		text="We accelerate ATO timelines by more than 50%, for some customers in as little as 90 days"
		check1="Classified & open environments"
		check2="70% NIST 800-53 Tech Control"
	/>
	<Card
		title="Deploy Anywhere"
		text="Defense Unicorns deliver mission capabilities wherever your mission requires"
		check1="cloud or on-prem"
		check2="Land, Air, Space, or Sea"
	/>
	<Card
		title="No Vendor Lock In"
		text="The Defense Unicorns platform baseline is open source, allowing for greater accessibility"
		check1="Infrastructure agnostic"
		check2="No Platform License"
	/>
</section>

<style>
	.section4 {
		display: flex;
		justify-content: space-evenly;
		align-items: center;
		flex-direction: row;
		position: relative;
	}

	.card-glow {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		z-index: -1;
	}

	@media (max-width: 1200px) {
		.section4 {
			flex-direction: column;
			gap: 3rem;
		}
	}
</style>
