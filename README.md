local-rich-snippets-bookmarklet
===============================

This bookmarklet requires jQuery. Simply drag it to your bookmark bar and click on it to send the current page's html code to Google's Rich Snippets tool. This is great for working with local files, instead of doing 1. View source 2. Select all 3. Copy 4. Close 5. New tab with the Rich Snippets tool 6. Paste ;-)

[Validate Local RichSnippet][1].

It requires jQuery!

[1]: javascript:(function()%7B(function()%7Bvar%2520htmlForm%3D'%3Cform%2520id%3D%22rstt-html-form%22enctype%3D%22multipart%2Fform-data%22method%3D%22POST%22'%3BhtmlForm%2B%3D'target%3D%22local_validator%22'%3BhtmlForm%2B%3D'action%3D%22http%3A%2F%2Fwww.google.com%2Fwebmasters%2Ftools%2Frichsnippets%2Fupload%22%3E'%3BhtmlForm%2B%3D'%3Ctextarea%2520name%3D%22html%22id%3D%22html-input%22%3EPaste%2520html%2520here.%3C%2Ftextarea%3E'%3BhtmlForm%2B%3D'%3C%2Fform%3E'%3B%24('body').append(%24(htmlForm))%3B%24form%3D%24('%23rstt-html-form')%3B%24textarea%3D%24('%23html-input')%3Bvar%2520fullHtml%3D%24('html').html()%3B%24textarea.val(fullHtml)%3B%24form.submit()%3B%7D)()%7D)()
