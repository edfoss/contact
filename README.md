# contact
Demonstration to see if a github/Mastondon link could be verified using just a README.md file.
This idea works well with another source code repository system.
Problem: the rel="me" attribute within the anchor tags is replaced with rel="nofollow" when the file is rendered in the browser which would probably confuse the Mastodon verification process.

<!--
<a rel="me" href="https://mstdn.social/@edfoss"></a>
<a rel="me" href="https://mstdn.social/@topics"></a>
<a rel="me" href="https://mastodon.social/@edfoss"></a>
<a rel="me" href="https://mastodon.online/@edfoss"></a>
-->

<pre>
&lt;a rel=&#34;me&#34; href=&#34;https://mstdn.social/@edfoss&#34;/&gt;
&lt;a rel=&#34;me&#34; href=&#34;https://mstdn.social/@topics&#34;/&gt;
&lt;a rel=&#34;me&#34; href=&#34;https://mastodon.social/@edfoss&#34;/&gt;
&lt;a rel=&#34;me&#34; href=&#34;https://mastodon.online/@edfoss&#34;/&gt;
</pre>
