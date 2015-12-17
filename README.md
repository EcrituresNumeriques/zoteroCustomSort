# zoteroCustomSort
quick function to sort zotero collection by custom tags, works with the web API (no authentification needed, but your collection needs to be accessible to the whole internet, works only in read mode).

This is a javascription fonction with the following structure:

zoteroPageSort([key of the collection], [with which value sort], [users|groups], [id of the users|groups]);


To use you need to 
 - include the zoteroPageSort.min.js (or the zoteroPageSort.js if you want to modify the function) either on the header, or above the call to the function.
 - include an element with the zoteroPageSort id where your data will be push to.


minimal example:

<pre><code>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;head&gt;
  &lt;meta charset="utf-8"&gt;
  &lt;title&gt;ZoteroPageSort&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;p id="zoteroPageSort"&gt;&lt;/p&gt;
&lt;script src="/link/to/your/zoteroPageSort.min.js"&gt;&lt;/script&gt;
&lt;script&gt;
zoteroPageSort("8U86CMSC", "firstPage", "groups","430843");
&lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;
</code></pre>
