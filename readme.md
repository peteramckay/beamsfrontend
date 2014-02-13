Beams
=========

Beams is a front-end Web framework designed primarily for multimedia-heavy sites. It should also integrate well with other types of Web projects that require beautiful display across different types of devices. 

Beams is free to use under MIT license. Key features of the framework so far: 

- Built in HTML5, CSS3, and jQuery. For the purposes of the current alpha version of Beams, the focus is really on the CSS3 piece. But there is an unmodified copy of jQuery v2.1.0 included as well just in case implementers need it, so they can put it on their servers and call it quicker for their applications. Will probably add other JavaScript enhancements later so that Beam becomes an even more of a full-fledged development tool.

- Responsive visual design based on a 20-column, 4,000-pixel grid -- approximately the physical screen size of a 48-inch TV. Yet the framework also scales down smoothly to any other size from desktop to tablet to smartphone as well.

- Default Roboto family typefaces from Google Fonts. Of coursre, implementers should feel free to change these to whatever else you want if necessary.

The basic building block of pages in the responsive layout is full-width containers with the class "beams" that act as rows to put several child elements in, like so...

	<div class="beam">
		<div class="ten">
			<!-- Some stuff here-->
		</div>
		<div class="eight">
			<!-- Some stuff here-->
		</div>
	</div> <!-- End of beam -->

The "beam" class may be applied to any type of element, but beams should all be children of the body element only. Nesting them any deeper in the DOM may cause the design to break.

The children of a beam can have classses of "one" to "twenty" to specify how many columns each should take up. Total widths of the he children should add up to no more than twenty, since that's how wide each beam is as the parent container.

Again, I consider this version of Beams an alpha. The framework here is still a bit rough around the edges, to be sure. But I think it's at least a good start, something to show to other developers, get feedback, and begin iterating quickly.

If you have any other feedback or suggestions, I'm glad to hear them via GitHub or email peteramckay@gmail.com.

Peter McKay | Feb. 12, 2014
