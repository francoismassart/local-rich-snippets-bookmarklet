local-rich-snippets-bookmarklet
===============================

This bookmarklet requires jQuery. Simply drag it to your bookmark bar and click on it to send the current page's html code to Google's Rich Snippets tool. This is great for working with local files, instead of doing 1. View source 2. Select all 3. Copy 4. Close 5. New tab with the Rich Snippets tool 6. Paste ;-)

[Validate Local RichSnippet][1].

It requires jQuery!

[1]: javascript:(function()%7Bfunction%20callback()%7B(function(%24)%7Bvar%20jQuery%3D%24%3Bvar%20htmlForm%3D'%3Cform%20id%3D%22rstt-html-form%22enctype%3D%22multipart%2Fform-data%22method%3D%22POST%22%20'%3BhtmlForm%2B%3D'target%3D%22local_validator%22'%3BhtmlForm%2B%3D'action%3D%22http%3A%2F%2Fwww.google.com%2Fwebmasters%2Ftools%2Frichsnippets%2Fupload%22%3E'%3BhtmlForm%2B%3D'%3Ctextarea%20name%3D%22html%22id%3D%22html-input%22%3EPaste%20html%20here.%3C%2Ftextarea%3E'%3BhtmlForm%2B%3D'%3C%2Fform%3E'%3B%24('body').append(%24(htmlForm))%3B%24form%3D%24('%23rstt-html-form')%3B%24textarea%3D%24('%23html-input')%3Bvar%20fullHtml%3D%24('html').html()%3B%24textarea.val(fullHtml)%3B%24form.submit()%7D)(jQuery.noConflict(true))%7Dvar%20s%3Ddocument.createElement(%22script%22)%3Bs.src%3D%22https%3A%2F%2Fajax.googleapis.com%2Fajax%2Flibs%2Fjquery%2F1.7.1%2Fjquery.min.js%22%3Bif(s.addEventListener)%7Bs.addEventListener(%22load%22%2Ccallback%2Cfalse)%7Delse%20if(s.readyState)%7Bs.onreadystatechange%3Dcallback%7Ddocument.body.appendChild(s)%3B%7D)()
