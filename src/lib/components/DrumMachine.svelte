<script lang="ts">
	const beats = {
		1: {
			enabled: false
		},
		2: {
			enabled: false
		},
		3: {
			enabled: false
		},
		4: {
			enabled: true
		},
		5: {
			enabled: false
		},
		6: {
			enabled: false
		},
		7: {
			enabled: false
		},
		8: {
			enabled: true
		},
		9: {
			enabled: false
		},
		10: {
			enabled: false
		},
		11: {
			enabled: false
		},
		12: {
			enabled: true
		},
		13: {
			enabled: false
		},
		14: {
			enabled: false
		},
		15: {
			enabled: false
		},
		16: {
			enabled: true
		}
	};
</script>

<section>
	{#each Object.keys(beats) as i}
		{@const beat = beats[i]}
		<div class="beat">
			<div class="beat__number">{i}</div>
			<div class="beat__toggle">
				<input type="checkbox" checked={beat.enabled} />
			</div>
		</div>
	{/each}
</section>
