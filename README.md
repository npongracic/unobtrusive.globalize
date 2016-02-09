# unobtrusive.globalize
This is a starter kit for anyone who wants to use asp.net's unobtrusive validation and globalize. 

###Why did i do this?
Because I can't believe it's so hard to even get globalize to run, there's like a million files you have to include if you're not a [npm|bower|insert client package manager] level90 dinowizard.

###What is this?
This project consists of:
 1. cldrjs + required globalize files combined together for your convenience so you only have to include one file
 2. Simple working culture file generated from the many confusing cldr-core, cldr-numbers-* etc. json files 
 3. Validation monkeypatch script from https://github.com/johnnyreilly/jquery-validation-globalize

Basically you only need to download these files and include them on your page somewhere after jquery and jquery.validation/jquery.unobtrusive, like so:

    <script src="~/lib/cldr.globalize.js"></script>
    <script src="~/lib/cultures/globalize.culture.hr.js"></script>
    <script src="~/lib/jquery.validate.globalize.js"></script>

And that's it.
I cant believe it's so hard to get this working.
