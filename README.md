browser-scripts
====================

Collection of small JavaScript functions and scripts that can be used in Firefox to interact with Lair

## Usage

1. Log into Lair.
2. If the script comments have "Requires client-side updates: true" you will need to turn on client updates, if not, you can skip this step. On the initial page under "Settings" ensure that you have enabled "client-side updates".
3. Load your desired project.
4. From within your browser, open your JavaScript console. How to do this is specific to your browser and/or plugins used.
5. Copy the script and/or function definition in its entirety; paste it into your JavaScript console.
6. Run the newly defined function, adhering to the usage defined in the comments of each script.

## Loading ALL Scripts

You can now import all_scripts.js or all_scripts_min.js in the developer console for easier access to all the browser scripts at once. 
Add the following as a bookmarklet by creating a new bookmark in your browser (I have it on my bookmark bar) with the location as:  

`javascript:(function() { $.getScript('https://cdn.jsdelivr.net/gh/6sp33d/lair-browser-scripts@master/all_scripts.js'); })();`

This will load all the scripts behind the scenes without having to remember the code snippet to do so.


### A couple notes regarding loading these scripts from URLs:

I specifically use the jsdelivr CDN because Firefox has content-type mismatches when using rawgit.com 

If you try to juse use the $.getScript() segment and put it into your developer console, you may have bad luck making it work. I never could, but somehow the bookmark always worked just fine. No idea what's up with that.
