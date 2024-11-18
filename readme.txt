This project is a script that takes ebooks (works best on epubs and html files) and converts them to pdfs optimized for printing: 8.5 by 11, small margins, small text, numbered pages, indents instead of double line breaks. This usually reduces the page count of the ebook by about half, saving paper. Be warned: If your eyesight is poor, you may find the text of the resultant pdfs uncomfortably small. A single page of a Coarse Ebook can contain over 1000 words!

This project requires calibre's convert-ebook to be installed. You can get it here: https://calibre-ebook.com/download

The books/ subdirectory of this project contains several pdfs produced by this script. Some of those pdfs have been massaged in some way beyond what the default script produces, and cannot be produced with the default script (TODO: is this still true as of 2024-11-18?). This irreproducibility is regrettable. Some of these pdfs have not been massaged at all, and thus are a bit crap, which is also regrettable.

replacements.txt contains lots of very specific replacements for specific books that are not applicable to other books. This is inelegant, but there's not much we can do about that; better to have them here than not.

I've lost the source file corresponding to "books/the meditations of the emperor marcus antoninus.epub.pdf", but it's probably from https://en.wikisource.org/wiki/The_Meditations_of_the_Emperor_Marcus_Antoninus or some equivalent source, somehow. Public domain, it seems.

Interested in my book-formatting github projects? These inescapable follies I've embroiled myself in? Well, I have three others:
* https://github.com/wyattscarpenter/unsong-book-fetcher/ (_Unsong_ by Scott Alexander)
* https://github.com/wyattscarpenter/terrorisland (_Terror Island_ by by Ben Heaton and Lewis Powell)
* https://github.com/wyattscarpenter/_why-the-lucky-stiff-printer-spool-2013 (_printer spool, 2013_ by _why the lucky stiff)
There may be more by the time you read this, but having made all those projects really makes me think: "it's not worth making more of these projects". There's also this related script I made, that basically just scrapes wordpress blogs to aid offline reading:
* https://github.com/wyattscarpenter/util/blob/master/scrape-wordpress.py

There are two bugs in convert-ebook we currently have to fight with: (1) if you don't put two line breaks before the page number it sometimes creates a completely blank page after a particularly full page (2) all images are written to the pdf as jpegs of diminished quality. Presumably these will be sorted out some day. (TODO: how's that looking as of 2024-11-18?)

The name of this project references the lack of polish in a book you print out yourself. The name is also a pointless reference to Horse_ebooks.

                       ,, ,,, ,,,, ,,,,,,,,
          /\        /;; ;;;;;;;;;;;;;; ;;;/ ,;`.   ,,,,
         ;  `-.    /// //////// /////  // ,','`;. ///;;;;,.
        ,'   ,,`-.;;;;;; ;;;;;;; ;;;;// ,' ,'  `.`. ///;;//;,
       ,'   ;;;//////// ////// ///////,'  ,'     ; : ;;// ;//,
       `.  ;`;;;;;;;: ;;;;:;; ;:;:;;:;:  ,'     ,' : ;;;;;;;;/,
        `. `; :!::::!;;;;;!::::!;!;;!;:  `.   ,'  ,'///!!;;;;;;
          `._!!;!!!!;!!!!!;!!!!;!;!!;!!`.  `;'  ,'-.!!!//;;;////
             ;   .   .               ,        ,'    ::-!_///;;;;
           .' ,%'  ,%'     `%.   `%.;;   `%.   ;;   ,::  `! ////
          .', '    '    `%,  `:.   `::.   ::  :;    %::    `! ;;
         ,';;        `%, `;;.         `::. `.;;;    `:%   %:///
        ,';;'  ;      ;;  `::;   `%,    ;%:.  ::     ::     %`!/
      ,' ;.'  .%.    ;;    `;;     ;;   ' `;   %     ::    %  :
      :  `;;  %%%    `::   ;;     ;;;      `    `    ::     % `
      ;    ' .%%'  `%  ;   '  ,., `;;         `%,   ::'   %::%
     ;`. `.  %%%%   ;;   .___;;;;  '     `:    `;   ::     :::
     : :  ;  %%%%   ;: ,:' _ `.`.        ;;;   ;;   `::    :::.
     `.;  ;  `%%'  ;;' :: (0) ; :       ::'    ;      ::   `:::
      ,' ;'  %%'  ;;'  ;;.___,',;       ;;    ;;       ;   ,:::
     ,  ;'  :%:   ;;  ,'------''      ;;;'  .;;            :::'
    ,' ;;   ;%;   ;;  '             ::'    ,;;;            :::
    :  :'   :%:   `;             ;;;;'      ;;             ::%
    :  ;;   :%'   ;;   ;...,,;;''         ;;'    ;     ;   :::
    ;  `;   ::   ;;' ,:::'     .        .;;     ,'    ;;   `;;
    ;  ;'   :: .;;' ,:::'   ,::%.      ;;;    ,'     ;;    ,;;
    : ;;.  .:' ;;' ,:::' ;;:::' ;;    ;;'    ,'    ;;;    ;;;'
     :`;;  ::  ;;  ;;;' '  .    ;;    '  _,-'     ;;;     `;'
     : ;' .:'  ;; .::: ,%'`;   ;;;   _,-'       .;;;'     ;'
    ,' ;; ;;  ;;' :::' ,, .;  ;;  _,' ;      ,;;;'     ,;;'
   .'~~~~~~~~~._ ,;' ,',' ;;  ',-'   ,'    ,';;       ;;;'   ;;;
 ,'             `-.,' .'  ;; ,'     ,' ;;;;;;'       ,;;    ;;;
.';           .    `.,   ;; ,'      ;              ,;;%    ;;;
: ..       _.';     ;   '_,'       .'       ,,,,,,,%;;'    `;;;
`.  .     (_.' .  ;'  ,-'          :  ,,,,,;;;;;;;;;'      .;;;
  `-._        ___,' ,'             :.."""""`````'        ,;;;;
      `------'____.'               :                   ..;;;;
         `---'                     `.               ..;;;;'
                                    :......:::::::::;;;;'
                                     :::::::::::::::;'      ,;;;
                                      ;                   ;;;;'
                                      ;                 .;;;;
                                    ,'...:::::.        ;;;'
                                   .'          `;;;;;;''
                                   ;
                                   `----------------------------

(I hope you enjoyed that coarse horse. I didn't make it, and unfortunately I don't know who did.)
