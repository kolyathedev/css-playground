<template>
	<header><h1>CSS Cheat Sheet</h1></header>
	<div class="left">
		Using Float Left with no other CSS will shrink the whole container to left of
		parent element, fitting content.
	</div>
	<div class="right">
		Using Float right with no other CSS will shrink the whole container to right
		of parent element, fitting content.
	</div>
	<div class="right-d-block">
		Using Float right with display block will shrink the whole container to right
		of parent element, fitting content. And place under sibling elements.
	</div>
	<div class="right-d-block">
		inline-block is ignored due to the float. If 'float' has a value other than
		'none', the box is floated and 'display' is treated as 'block'
	</div>
	<div class="main">
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam unde rerum
		temporibus tenetur quaerat nam, neque tempore explicabo minima voluptatum
		laboriosam nihil non nesciunt magnam accusantium hic, deleniti, dicta
		distinctio.
	</div>

	<div class="col-xs-1"></div>
	<div class="col-xs-2"></div>
	<div class="col-xs-4"></div>
	<div class="col-xs-5">
		No Row Tag Nest. Screens smaller than 600px will revert to col val, otherwise
		100%. <b>col-xs-</b>
	</div>
	<div class="row">
		<div class="col-1"></div>
		<div class="col-2"></div>
		<div class="col-4"></div>
		<div class="col-5">
			With Row Tag. Height different because of padding. <b>col-</b>
		</div>
	</div>
	<div class="row">
		<div class="col-s-1"></div>
		<div class="col-s-2"></div>
		<div class="col-s-4"></div>
		<div class="col-s-5">
			With Row Tag. With break point for screens larger than 600px, as we design
			mobile first. <b>col-s-</b>. That is, will break to col values after 600px,
			but less will be 100% width.
		</div>
	</div>
	<div class="row">
		<div class="col-m-2"></div>
		<div class="col-m-1"></div>
		<div class="col-m-5">
			With Row Tag. With break point for screens larger than 768, as we design
			mobile first. <b>col-m-</b>. That is, will break to col values after 768px,
			but less will be 100% width.
		</div>
		<div class="col-m-4"></div>
	</div>
	<div class="row">
		<div class="col-lg-2"></div>
		<div class="col-lg-1"></div>
		<div class="col-lg-5">
			With Row Tag. With break point for screens larger than 992, as we design
			mobile first. <b>col-lg-</b>. That is, will break to col values after 992px,
			but less will be 100% width.
		</div>
		<div class="col-lg-4"></div>
	</div>
	<div class="row">
		<div class="col-xl-5">
			With Row Tag. With break point for screens larger than 1200, as we design
			mobile first. <b>col-xl-</b>. That is, will break to col values after 1200px,
			but less will be 100% width.
		</div>
		<div class="col-xl-2"></div>
		<div class="col-xl-1"></div>
		<div class="col-xl-4"></div>
	</div>
	<div class="row">
		<div class="col-m-12 hide-orientation-land">
			This will be hidden in landscape orientation!
		</div>
	</div>
	<div class="row">
		<div class="col-m-5">5</div>
		<div class="col-m-4">
			4
			<img src="../assets/logo.png" alt="logo" />
		</div>
		<div class="col-m-1">1</div>
	</div>
	<div class="flex-container" title="flex-box">
		<div style="flex-grow: 1; order: 3">Flex child order 3, flex grow</div>
		<div style="flex-grow: 1; order: 1; align-self: flex-end">
			order 1, align self flex end
		</div>
		<div style="flex-grow: 1; order: 2; align-self: center">
			order 2, align self center
		</div>
		<div style="flex-grow: 3; order: 4; align-self: flex-start">
			order 4, align self flex start, flex grow 3
		</div>
	</div>
	<div
		class="grid-container-block"
		title="grid-container with display: grid (left as block container)"
	>
		<div class="item-1">Block display grid container</div>

		<div class="item-2">css {display: grid;}</div>
		<div class="item-3">
			The display prop specifies the display behavior (the type of rendering box of
			an element)
		</div>
		<div class="item-4">
			Displays an element as a block element (like &lt;p> ). It starts on a new
			line, and takes up the whole width.
		</div>
		<div class="item-5">
			The items have been split into two columns of auto width {
			grid-template-columns: auto auto;}
		</div>
		<div class="item-6">6</div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
	<div class="grid-container-inline">
		<div class="item-1">A grid container with display set to Inline-grid.</div>
		<div class="item-2">2</div>
		<div class="item-3">3</div>
		<div class="item-4">4</div>
		<div class="item-5">5</div>
		<div class="item-6">6</div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
	<div class="grid-container-1">
		<div class="item-1">
			A grid container with display set to grid. Each element constrained to 1fr of
			10 in cols.
		</div>
		<div class="item-2">grid-template-columns: repeat(10, 1fr);</div>
		<div class="item-3">3. Will extend in height to maintain this.</div>
		<div class="item-4">4</div>
		<div class="item-5">5</div>
		<div class="item-6">6</div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
	<div
		class="grid-container-2"
		title="10 rows only set to 1fr each(one fraction of available height of container)"
	>
		<div class="item-1">
			A grid container with display set to grid. Each element constrained to 1fr of
			10 in rows.
		</div>
		<div class="item-2">grid-template-rows: repeat(10, 1fr);</div>
		<div class="item-3">3</div>
		<div class="item-4">4</div>
		<div class="item-5">5</div>
		<div class="item-6">6</div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
	<div
		class="grid-container-3"
		title="10 rows only set to 1fr each(one fraction of available height of container)"
	>
		<div class="item-1">A grid container with display set to grid.</div>
		<div class="item-2"><b> grid-template-columns: repeat(10, auto);</b></div>
		<div class="item-3">
			With each col width set to auto, it fits the max width of the child first,
			rather than above where the content is constrained to the grid container
			column width declaration.
		</div>
		<div class="item-4">4</div>
		<div class="item-5">5</div>
		<div class="item-6">6</div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
	<div
		class="grid-container-4"
		title="container 4 : 10 rows only set to 1fr each(one fraction of available height of container) "
	>
		<div class="item-1 col-m-12">A grid container with display set to grid.</div>
		<div class="item-2">
			<b> grid-template-columns: repeat(10, 1fr) after 1200px.</b>
		</div>
		<div class="item-3">
			grid-template-rows: repeat(10, auto); less than 1200px Note I have rid the
			columns! So these now stack and fit the content
		</div>
		<div class="item-4">
			That is, on small devices, adjust column width to max-content(I think)
		</div>
		<div class="item-5">
			What's causing the horizontal scroll is are the grids set to
			grid-template-columns: repeat(10,1fr)
		</div>
		<div class="item-6">6</div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
	<div
		class="grid-container-5"
		title="Same as above but with default setting to repeat(10,1fr)"
	>
		<div class="item-1">A grid container with display set to grid.</div>
		<div class="item-2"></div>
		<div class="item-3">
			grid-template-rows: repeat(10, 1fr); less than 1200px Note I have rid the
			columns! So these now stack and but are all of equal row height.
		</div>
		<div class="item-4">
			Interesting that as you re-size the screen and the conent wraps, all grid
			items get higher to ensure 1fr/10 is maintained.
		</div>
		<div class="item-5">
			<b
				>An interesting note. Here I set the background setting as template rows to
				repeat 10 1fr, and then change the grid-template-columns after 1200 px, but
				after 1200px the grid-template-rows is still in effect as I have not removed
				it!
			</b>
		</div>
		<div class="item-6">Hence the massive white space underneath....</div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
	<div
		class="grid-container-6"
		title="Same as above but with default setting to repeat(10,1fr)"
	>
		<div class="item-1">A grid container with display set to grid.</div>
		<div class="item-2">
			<b>grid-template-columns: repeat(10, 1fr) after 1200px.;</b>
		</div>
		<div class="item-3">
			grid-template-rows: repeat(10, 1fr); less than 1200px Note I have rid the
			columns! So these now stack and but are all of equal row height.
		</div>
		<div class="item-4">
			Interesting that as you re-size the screen and the conent wraps, all grid
			items get higher to ensure 1fr/10 is maintained.
		</div>
		<div class="item-5">(5) grid-column: 3 / span 2;</div>
		<div class="item-6">6</div>

		<div class="item-7">(7) grid-column: 1 / span 4;</div>
		<div class="item-8">8</div>
		<div class="item-9">(9) grid-column: 7 / span 3;</div>
		<div class="item-10">
			(10) When adjusted for specific item col/row spans, will break order and then
			continue. Will mess up at lower break points to maintain container defined
			order and item placement.
		</div>
	</div>
	<div
		class="grid-container-7"
		title="Grid container, display grid, +1200 break to 10 cols auto and justify-content center"
	>
		<div class="item-1">A grid container with display set to grid.</div>
		<div class="item-2">After 1200 gtc: r(10,auto)</div>
		<div class="item-3">Default; justify-content start</div>
		<div class="item-4">After 1200, justify-content center</div>
		<div class="item-5"></div>
		<div class="item-6"></div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
	<div
		class="grid-container-8"
		title="Grid with 5 cols 1fr 3 rows 1fr , grid-auto-flow: column "
	>
		<div class="item-1">1</div>
		<div class="item-2">2</div>
		<div class="item-3">3</div>
		<div class="item-4">4</div>
		<div class="item-5">5</div>
		<div class="item-6">6</div>
		<div class="item-7">7</div>
		<div class="item-8">8</div>
		<div class="item-9">9</div>
		<div class="item-10">10</div>
	</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
	name: 'HomeView',
})
</script>
