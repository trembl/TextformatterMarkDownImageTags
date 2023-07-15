Problem:
I am a building a site, that relies on _TextArea + Markdown/Parsedown Extra_ for it main content field. How to add images to the text? Uploading images with an _Image_ field works, but how to expose the URL and get it into the Markdown?

After diving deeping into the Image Field, I came across [this method](https://github.com/ocorreiododiogo/PW-ImageTags). Images from an image field get inumerated, and short-codes can be added to the textarea. Nearly exactly what I want. Nearly.

Instead of outputting `<img src="...`, it would be enough to just get the image URL - and then use the Markdown Image Link to make the HTML, if necessary with additional Parsedown.

`![]({images:1}){.w-50}`


## Text Formatter Order
1. Image Tags
2. Markdown/Parsedown Extra


Original documentation at [https://github.com/ocorreiododiogo/PW-ImageTags/](https://github.com/ocorreiododiogo/PW-ImageTags)
