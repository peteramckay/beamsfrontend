Beams
=========

Beams is a front-end Web framework designed primarily for multimedia-heavy sites. It should also integrate well with other types of Web projects that require beautiful display across different types of devices. 

Beams is free to use under MIT license. Key features of the framework so far: 

- Built in HTML5, CSS3, and jQuery. For the purposes of the current alpha version of Beams, the focus is really on the CSS3 piece. But there is an unmodified copy of jQuery v2.1.0 included as well just in case implementers need it, so they can put it on their servers and call it quicker for their applications. We may add other JavaScript enhancements later so that Beam becomes an even more of a full-fledged development tool.

- Responsive visual design based on a 20-column, 4,000-pixel grid -- approximately the physical screen size of a 48-inch TV. Yet the framework also scales down smoothly to any other size from desktop to tablet to smartphone as well.

- Default Roboto typefaces from Google Fonts. Of coursre, implementers should feel free to change to whatever else you want.

The basic building block of pages in the responsive design is full-width containers with the class "beams" that basically act as rows to put several child elements in, like so...

	<div class="beam">
		<div class="ten">
			<!-- Some stuff here-->
		</div>
		<div class="eight">
			<!-- Some stuff here-->
		</div>
	</div> <!-- End of beam -->

The "beam" class may be applied to any element, but beams should all be children of the body element only. Nesting them any deeper in the DOM may cause the design to break.

The children of a beam can have classses of "one" to "twenty" to specify how many columns each shoudl take up. Please note, although each beam is 20 columns wide, the children's widths should add up to no more than 18. This is because there's about a column's worth of whitespace on the side of each div by default.

Please note, Beams suite is currently at v0.1, an alpha release. The framework here, as well as some complementary modules for server configuration and ad display, are still a bit rough around the edges, to be sure. But we believe we at least have a good start here, something we can show to other developers, begin to build a community around, and begin iterating quickly.

Will certainly be adding integration with, Vimeo and Kaltura APIs for video players, etc, in short order. Of course, we're going to need that for the sake of video integration. If you have any other feedback or suggestions, I'm glad to hear them via GitHub or email peteramckay@gmail.com.

Peter McKay
Feb. 10, 2014
