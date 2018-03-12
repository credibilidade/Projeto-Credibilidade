# Edge Side Includes
One light-weight way of including site-level metadata into your HTML can be Edge-Side-Includes.

This is a not yet standardized way of "including" stuff from other servers into your websites. This option can solve a problem if access to the templates for the generated HTML is not easily possible and / or if the system used to update the site-wide metadata is decoupled from the CMS. By including a tag like the one below, you can "include" the markup in the page.

<esi:include src="http://example.com/site-wide-trust-project-markup-v1.1.json" onerror="continue"/>

It's documented quite reasonably <a href="https://en.wikipedia.org/wiki/Edge_Side_Includes">in the Wikipedia article</a>. It is ony advisable to consider using Edge Side Includes if you have the builing blocks that support it already in your infrastructure: either a supporting caching proxy servers such as Varnish, Squid and Mongrel ESI or the services of a Content Delivery Network such as Akamai or Cloudflare.

This "include" paradigm also can work on the server (please google Server Side Includes).

ATENÇÃO: Conteúdo original desta página <a href="https://github.com/TheTrustProjectCode/Trust-Project-Schema.org-Markup-Examples-2017/blob/master/Newsrooms/site%20level/dpa-edge-side-include-note.md">disponível aqui</a>
