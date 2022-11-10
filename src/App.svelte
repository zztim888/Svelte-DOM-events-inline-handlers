<script>
	let m = { x: 0, y: 0 };

  // with inline handlers("{e => m={x: e.clientX, y: e.clientY}}") 
  // that code below can be commented

	// function handleMousemove(event) {
	// 	m.x = event.clientX;
	// 	m.y = event.clientY;
	// }
</script>
<!-- this is one way writing the code -->
<!-- <div on:mousemove={handleMousemove}>
	The mouse position is {m.x} x {m.y}
</div> -->

<!-- and this is another way -->
<!-- inline handlers -->
<div on:mousemove="{e => m={x: e.clientX, y: e.clientY}}">
	the mouse position is {m.x} x {m.y}
</div>

<style>
	div { width: 100%; height: 100%; }
</style>