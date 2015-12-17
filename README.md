# zoteroCustomSort
quick function to sort zotero collection by custom tags, works with the web API (no authentification needed, but your collection needs to be accessible to the whole internet, works only in read mode).

This is a javascription fonction with the following structure:

zoteroPageSort([key of the collection], [with which value sort], [users|groups], [id of the users|groups]);


To use you need to 
 - include the zoteroPageSort.min.js (or the zoteroPageSort.js if you want to modify the function) either on the header, or above the call to the function.
 - include an element with the zoteroPageSort id where your data will be push to.


minimal example:


<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>ZoteroPageSort</title>
</head>
<body>
<p id="zoteroPageSort"></p>
<script src="zoteroPageSort.js"></script>
<script>
zoteroPageSort("8U86CMSC", "firstPage", "groups","430843");
</script>
</body>
</html>
