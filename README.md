John Bolibol

1. I would fit my automated tests within a Github action that runs whenever code is pushed. This way I would somewhat know what version of the software or what changes broke the software that caused the failure. It helps me catch bugs early thus saving me time compared to manually running tests. It also helps keep the project stable throughout the development.

2. No.
   
3) Navigation mode starts the webpage from the beginning and tests how well it loads. It checks things like speed and performance during the loading process. Snapshot mode looks at the webpage in its current state without reloading it. It is mainly used to inspect accessibility, SEO, and page structure.

4) 
   - According to Lighthouse "<html> element does not have a [lang] attribute", maybe we can add an HTML tag that specifies a language so browsers can use that to know the language of the page. We can probably use a faster server response and host the site on a faster platform other than github pages
   - Lighthouse gave the error, "Document request latency." This means the first request to load the page responded slower than what was expected. According to Google, this can be fixed by avoiding redirects and enabling text compression. Moreover, text compression reduces the size of files like HTML, CSS, and JavaScript before they are sent to the browser. Smaller files download faster and improve loading speed.
   - According to Lighthouse, we should "Use efficient cache lifetimes." The caches are only being stored for 10 minutes. The site is not reusing the files but redownloading them when someone is visiting multiple times. We could increase cache lifetime so that files are stored in the browser longer. This should reduce loading times. 




