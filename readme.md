# Google Docs Shortcode #

Google Docs Shortcode is a small plugin for WordPress that allows you to use a [shortcode](https://codex.wordpress.org/Shortcode) to easily embed a Google Doc into your blog posts or pages.

The shortcode supports the following Google Doc formats:
* Documents
* Presentations
* Spreadsheets
* Forms

This plugin was developed for the [CUNY Academic Commons](http://commons.gc.cuny.edu).  Licensed under the GPLv2 or later.

***

### How to Use

#### Embedding a document, presentation or spreadsheet
1. First, you�ll need to find the public URL of your Google Doc. Let's start by [logging in to your Google Docs](https://docs.google.com). Next, find the item you want to embed.
2. You should now have your Google Doc open.  Next, navigate to "**File > Publish to the Web**". A dialogue box should appear, similar to the one below:  
![Publish to the Web dialog window](http://codex.commons.gc.cuny.edu/files/2012/08/googledocs.jpg)  
3. Make sure that the "**Automatically republish when changes are made**" checkbox is checked. This will allow you to make changes to your Google Docs and have these changes automatically reflected on your WordPress site.
4. Copy the "**Document Link**" highlighted in red above.
5. Now navigate to your WordPress dashboard and open up the post or page where you want to embed your document. On a new line, type the following shortcode and paste in the link you copied, above:

  <pre>[gdoc link="THE LINK YOU COPIED" height="800"]</pre>
    
You can customize the shortcode by using [some custom parameters mentioned below](#other-shortcode-parameters).

#### Embedding a form
1. Follow steps 1-3 above.
2. Next, navigate to "**Form > Go to live form**".  This should take you to the public version of the form.  Copy the URL from your browser's address bar.
3. Follow step 5 above.

***

### Other shortcode parameters

Here are some other custom parameters you can use with the shortcode:

* "width" - By default, this tries to use your theme's content width. If this doesn't exist, the width is "100%". Fill in this value to enter a custom width.

* "height" - Enter in a custom height for your Google Doc if desired. Defaults to "300". Avoid percentages.

* "seamless" - This parameter is only applicable to Documents. If you enter "0", this will show the Google Docs header and footer.  Default value is "1", which means that no Google Docs header or footer will be shown.

* "size" - This parameter is only applicable to Presentations.  You can enter in "small", "medium" or "large" to use the presentation preset sizes. Dimensions for these presets are: small (480x389), medium (960x749), large (1440x1109). To set a custom width and height, use the "width" and "height" parameters listed above instead.

***

### Thanks

* Scott Voth - for testing and writing a version of this documentation on the CUNY Academic Commons codex.
* Christopher Stein - for noting a bug about using older presentations with the plugin.