Contributors: heinzcooler
Donate link: http://www.heinzcooler.de/
Tags: category, header
Requires at least: 2.8
Tested up to: 2.8
Stable tag: 1.03

This Wordpress Pluging lets you insert a different header for every category or tag page.

== Description ==

Normaly there is no introducing text at the category/tag page and so there is no interesting content for google.
Now you can edit at an optionpage for every category/tag an extra header, which is shown at the category/tag page.


== Installation ==
After activating the plugin you have to insert `<?= get_chc(); >` in your category template, to find at category.php in your
template directory. If there is no category.php (like in Kubrick) look out for archive.php and column 
`<?php /* If this is a category archive */ if (is_category()) { ?>
		<h2 class="pagetitle"><?php printf(__('Archive for the &#8216;%s&#8217; Category', 'kubrick'), single_cat_title('', false)); ?></h2>`
and insert `<?= get_chc(); >` directly after this, or wherever you want.

For the "Tag Header" you have to insert `<?= get_thc(); >` in your tag template, to find at archive.php in the template directory.
Shortly after  if (is_tag()) { 

== Frequently Asked Questions ==

= Are there some questions already? =

No.

== Screenshots ==


