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


<a rel="me" href="https://mstdn.social/@edfoss"></a>

<!--
<a rel="me" href="https://mstdn.social/@edfoss"></a>
<a rel="me" href="https://mstdn.social/@topics"></a>
<a rel="me" href="https://mastodon.social/@edfoss"></a>
<a rel="me" href="https://mastodon.online/@edfoss"></a>
-->
