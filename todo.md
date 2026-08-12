#####
#####

** check about and resources page for grammar

* add suggestion button to content menu

* coding/latex section: more advice than links,
- for simple latex use overleaf and for larger files or more complex scenarios use vscode with miktex and tex extension (course aswell...)
- vscode how to setup, install python (direct links) (basic setup videos)

* change main text size, and other sizes to either pixel width, vw, and use child text sizes with em/rem so that its relative to parents size/root size

* on homepage get logo and phy-hub text to be centered on top half of screen and change scaling of class="banner" to scale better for phones, and layout in general to be better for phones, i.e. stack links instead of having them side by side

#####
#####













* when page is thin, there is overflow to righthand side









### formating:

* use .hide() .show() Instead of manually setting the style attribute with .attr(), in bottom javascript
* make logo svg ( python script, miniturise, see if gzipping it is possible when being used) (i already have roof and stairs svg on SR handbook page)


### css/style:
* use same font size as wikipedia
* maybe have title svg and part by itself with a begin > button * bt need to remove references (possibly only have used refs in parts/chapters load, would need to have extra tag/info on bibs)
* next/previous button brings up to book title instead of chapter, also they never load parts

### sidebars:
### checks:
* some equations have too many terms in sidebar

### html tips:
* use em to size relative to parents font size, or rem which is relative to root font size, this can help get rid of need for media quiery
* can use p { width: clamp(45ch, 50%, 75ch); } to make paragraphs width in content min 45 character length and max 75ch and prefered 50%
* create variables for things such as navbar hieght and padding, you set the variable as global with :root { --VarName: value; } and call it using for example height: var(--VarName);

* change scrollbar using ::-webkit-scrollbar (make sure webkit is not just for chrome)
* use PostCSS to to make sure css is same throughout different browsers

* use float property instead of grid or flexgrid
* margin: auto centres element blocks vertically and horizontally
* for text, text-align: center;
* center divs inside a tag vertically using .ClassName {display: flex; align-items: centre; justify-content: center; } or do it using .ClassName { * display: grid; place-items: center; }

### mobile version:
* ...

### latex:
* appendix
* have a summary page with main equations
* express that time slowing and length contraction not being an optical illsuion, or is it ?
* posiibly use bibtex2html for references (  swap bibtex-js for own coded option, or Citation.js if needed)
* \cite{einstein1905electrodynamics} and \cite{SRtestsWiki,SRtestsUniCR} are numbered wrong in latex bibliography


*************************************************************************
*************************************************************************
things to do (MUCH LATER):
*************************************************************************
*************************************************************************
* think of better way for mobile users to get TOC on screen   <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">    <line x1="8" y1="6" x2="18" y2="6"></line> <line x1="8" y1="12" x2="18" y2="12"></line><line x1="8" y1="18" x2="18" y2="18"></line><line x1="3" y1="6" x2="3.01" y2="6"></line><line x1="3" y1="12" x2="3.01" y2="12"></line><line x1="3" y1="18" x2="3.01" y2="18"></line></svg>
* automate removal of background colour of tikz svg images i.e. the element with fill:#ffe4c8;
* The angstrom sign is normalized into U+00C5 Å LATIN CAPITAL LETTER A WITH RING ABOVE (HTML entity &Aring;, &#xC5;, or &#197;)




pages:

* patreon/donate page
* resources page for each topic (video/playlists, books, websites, for different topics and math pages)
* cosmythos story
* questions and thoughts in physics (with disclaimer)
* page on scientific biases to avoid
* historical journey
* merchandise
* physics overview page


html to continue doing:
* keep using hls instead or rgb for easier colour choices





*** my code setup:

- github
- git
    - winget install --id Git.Git -e --source winget

- python 3.12.4
    - winget install --id Python.Python.3.12.4 -e --source winget --scope user

- miktex

- strawberry perl
    - winget install StrawberryPerl.StrawberryPerl

- pdf2svg
    - git clone https://github.com/jalios/pdf2svg-windows.git pdf2svg
    - add C:\pdf2svg\dist-64bits; to PATH

- svgo (makes svg files smaller)
    - git clone https://github.com/svg/svgo.git svgo
    or
    - winget install OpenJS.NodeJS.LTS
    - npm install -g svgo


- GPL ghostscript (to minify pdfs)

- Inkscape
    - winget install -e --id Inkscape.Inkscape
    - add to path C:\Program Files\Inkscape\bin

- pip install playwright
- python -m playwright install
- playwright install chromium

- pip install beautifulsoup4
