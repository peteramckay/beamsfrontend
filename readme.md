#Beams Front End (v0.1.0)

Beams Front End is a responsive HTML5/CSS3 layer built for media-rich projects like news sites, video-heavy web apps, blogs, and so on. It's part of the full-stack Beams development framework, which also includes a server module and ad plugin.

All the Beams modules were created by me on behalf of Roscoe Labs. They're free to use under MIT license. 

For a fuller introduction to Beams, visit http://roscoelabs.com/products/beams or http://github.com/roscoelabs

Please note, we do consider this version of the front-end module to be an alpha release. We're eager to develop a community around the software to keep improving it from here. In that spirit, we welcome contributions of all kinds via GitHub, including forks, pull requests, bug reports, feature suggestions, and so on.

There's also a Beams Working Group email list that anyone can join at https://groups.google.com/forum/#!forum/beams-working-group

Now, on to some specifics about the front-end module. I'll admit, I'm more or less a Node.js newbie, so I'm going to cover a lot of basics here...



###Features

- Built in HTML5, CSS3 and jQuery v2.1.0. Repo includes its own copy of jQuery so implementers can access all its features quickly for their projects, as well as the plugin FitVids.js, which specifically helps with responsive scaling of video players.

- Responsive visual design in CSS3 based on a 20-column, 4,000-pixel grid -- approximately the physical screen size of a 48-inch TV. Yet the framework also scales down smoothly to any other size from desktop to tablet to smartphone as well.

- Default Roboto family typefaces from Google Fonts. Of course, implementers should feel free to change these to whatever else you want if necessary.


###Usage

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

The children of a beam can have classses of "onecolumn" to "twentycolumn" to specify how many columns each should take up. Total widths of the children should add up to no more than twenty, since that's how wide each beam is as the parent container.

There are also a few specialized CSS classes to quickly cover many effects that designers frequently use. For instance, a .centered class to automatically center a child element within a parent. Other examples include .unpadded, .padded-top, .padded-bottom, etc. For a full list, check out the "miscellaneous" section of the main layout.css file.

CSS styles are spread across three stylesheets, one that has the basic layout, including the responsive grid; one that includes media queries; and one that's blank for users to write custom styles for their particular projects.

Again, I consider this version of Beams Front End an alpha. The framework here is still a bit nascent, to be sure. But I think it's at least a good start, something to show to other developers, get feedback, and begin iterating quickly.

Peter McKay   
Co-Founder/Chief Product Officer   
Roscoe Labs   
April 2, 2014   

