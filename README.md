# contact
Demonstration to see if a github/Mastondon link could be verified using just a README.md file.
This idea works well with another source code repository system.
Problem: the rel="me" attribute within the anchor tags is replaced with rel="nofollow" when the file is rendered in the browser which would probably confuse the Mastodon verification process.  
An anchor element looks like the following line in the file

`<a rel="me" href="https://mstdn.social/@edfoss"></a>`

No joy: Try enclosing the block of anchors with a code block delimited by triple back-tics.

No joy: Try enclosing one anchor within single back-tics.

Note that the following link would work as expected with Mastodon verification  
https://gitlab.com/edfoss/contact/-/raw/main/README.md  
but looked like heck.

So perhaps the next thing to try is creating a readme.html file and using a raw view mode.

Result: verification works but when the page is opened from Mastodon in another tab it resembles a plain text file with no clickable links (does half of what is required). This approach is not much better than viewing the README.md file in raw mode.  
A wordpress blog is easier to setup for most people who are not familiar with github markdown.  
Doubtful if github markdown language was setup for what I want to do.

Note that a github profile seems to have [not enough for me] four spots for social media accounts which seems to permit verification to work with Mastodon.

&lt;a rel=&QUOT;me&QUOT; "https://mstdn.social/@edfoss" &gt;GenericAccount&lt;/a&gt;  
&lt;a rel=&QUOT;me&QUOT; &QUOT;https:&sol;&sol;mstdn.social&sol;@topics&QUOT; &gt;Topics&lt;&sol;a&gt;


<!--
<a rel="me" href="https://mstdn.social/@edfoss">Contact</a>
<a rel="me" href="https://mstdn.social/@edfoss"></a>
<a rel="me" href="https://mstdn.social/@topics2"></a>
<a rel="me" href="https://mastodon.social/@edfoss"></a>
-->
