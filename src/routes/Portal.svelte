<script>
	let { children } = $props();

	function portal(node) {
		function update() {
			document.body.appendChild(node);
			node.hidden = false;
		}

		function destroy() {
			if (node.parentNode) {
				node.parentNode.removeChild(node);
			}
		}

		update();

		return {
			update,
			destroy
		};
	}
</script>

<div use:portal hidden>
	{@render children()}
</div>
