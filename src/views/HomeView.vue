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
	<div class="flex-container">
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
	<div class="grid-container-block">
		<div class="flex-item item-1">Block display grid container</div>

		<div class="flex-item item-2">css {display: grid;}</div>
		<div class="flex-item item-3">
			The display prop specifies the display behavior (the type of rendering box of
			an element)
		</div>
		<div class="flex-item item-4">
			Displays an element as a block element (like &lt;p> ). It starts on a new
			line, and takes up the whole width.
		</div>
		<div class="flex-item item-5">
			The items have been split into two columns of auto width {
			grid-template-columns: auto auto;}
		</div>
		<div class="flex-item item-6">6</div>
		<div class="flex-item item-7">7</div>
		<div class="flex-item item-8">8</div>
		<div class="flex-item item-9">9</div>
		<div class="flex-item item-10">10</div>
	</div>
	<div class="grid-container-inline">
		<div class="flex-item item-1">
			A grid container with display set to Inline-grid.
		</div>
		<div class="flex-item item-2">2</div>
		<div class="flex-item item-3">3</div>
		<div class="flex-item item-4">4</div>
		<div class="flex-item item-5">5</div>
		<div class="flex-item item-6">6</div>
		<div class="flex-item item-7">7</div>
		<div class="flex-item item-8">8</div>
		<div class="flex-item item-9">9</div>
		<div class="flex-item item-10">10</div>
	</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
	name: 'HomeView',
})
</script>
