EDM-guideline
=============

Par pontban megprobaltam osszeszedni, hogy mi az, ami kell egy edm elkeszitesehez, mi a jo irany, es mihez kellene magatokat tartani.

Mellekletben talaltok egy template-t, amit ezen iranyelvek alapjan keszitettem. 

####Par szoban errol a template-rol:
 * index.html - ez mar a 'leforditott' markup, inline style
Tanulmanyozni, felhasznalni, modositani nyugodtan.
 * index-source.html - ez a forrasfajl, ezt forditod le mindig, itt nem kell inline css.

###Template

 * http://zurb.com/ink/
 * http://htmlemailboilerplate.com/

###Leiras

 * http://templates.mailchimp.com/development

###Tamogatottsag

 * http://www.campaignmonitor.com/css/

###Tesztelni
 * https://litmus.com/ - ez egy online tool, ami preview-t general az altalad hozaadott template-bol
 * http://putsmail.com/ - az altalad beillesztett templatet emailben el tudod kuldeni barkinek

###Roviden
 * css-t az html tagekhez inline kell irni, mivel nem minden kliens (gmail) tamogatja ezt. ettol fuggetlenul bent lehet hagyni, de az inline ugyis erosebb lesz, igy az lep majd ervenybe.
 * Bekezdesek vannak (kellenek is), lehet adni nekik margin-t is
 * Bal es jobb oldali behuzasokat vagy spacer elemekkel oldod meg, vagy tobb tablazatot agyazol egymasba (ez jo irany), amivel azt ered el, mintha lenne egy container elemed, ami pl: *970px szeles es margin: 0 auto-val kozepre van igazitva. tablazat eseteben nyilvan kozepre igazitott szoveg, majd a beagyazott tablazatnal balra igazitas*
 * Kepek sima kepek, szelesseg es magassag megadasa kell. illetve egy minimalis fix kell meg, hogy blokkositod oket
 * Alt es title attributumokat ki kell tolteni
 
###Inline styler

 * http://beaker.mailchimp.com/inline-css - headben definialt style-bol kiszedi a css ruleokat, es a selectornak megfelelo elemhez inline stylekent beilleszti.
 * https://pypi.python.org/pypi/inlinestyler
 
###Miert eri meg kulon fajlba/egy style tagbe irni a css, es nem egybol inline?
 * Mert nem 10 helyen kell modositanod
 * Atlathatobb lesz a build
 * **Mert meno**