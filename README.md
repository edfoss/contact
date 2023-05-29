# contact
Demonstration to see if a github/Mastondon link could be verified using just a README.md file.
This idea works well with another source code repository system.
Problem: the rel="me" attribute within the anchor tags is replaced with rel="nofollow" when the file is rendered in the browser which would probably confuse the Mastodon verification process.
Try enclosing the block of anchors with a code block delimited by triple-back-tics.

```
<a rel="me" href="https://mstdn.social/@edfoss"></a>
<a rel="me" href="https://mstdn.social/@topics"></a>
<a rel="me" href="https://mastodon.social/@edfoss"></a>
<a rel="me" href="https://mastodon.online/@edfoss"></a>
```
