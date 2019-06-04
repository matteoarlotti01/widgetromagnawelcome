Widget Emilia Romagna Welcome
========

Per usufruire del widget di prenotazione Experience di Romagna Welcome c'è la possibilità di usufruire di più modalità.

- Modalità nuova pagina 
- Modalità <iframe>
- Modalità fancybox (richiede javascript)

Ogni widget, è disponibile in lingue tradotte:

- Italiano
- Inglese
- Francese
- Tedesco

Modalità nuova pagina
----------
Effettuare link ad una nuova pagina, al seguente URL:

- https://experience.romagnawelcome.it/

Sarà possibile appendere il codice lingua per le traduzioni (https://experience.romagnawelcome.it/en): 

- /en
- /fr
- /de

Modalità <iFrame>
----------
E' possibile inglobare all'interno di una pagina del sito web dell'hotel, la pagina di prenotazione delle Experience, tramite inserimento <iframe>
.. parsed-literal::
        <iframe id="romagnaWelcome" src="https://experience.romagnawelcome.it/it/" frameborder="0" width="100%"></iframe>
Per modificare la lingua di caricamento, sostituire ``/it/`` con:  ``/en/``, ``/fr/`` o ``/de/``

Modalità fancybox
----------
La modalità fancybox consente di aprire un widget in overlay sul sito, che permette al visitatore di prenotare e concludere l'acquisto senza abbandonare il sito web dell'hotel:

.. parsed-literal::
        <a href="#" id="trekksoft_1727"><img src="https://experience.romagnawelcome.it/cache/images/widget-buttons/eyJsYWJlbCI6Ilwvd2lkZ2V0XC9ib29rLWJ1dHRvbi5wbmciLCJjYXB0aW9uIjoiQWNxdWlzdGEgbGUgRXhwZXJpZW5jZSBkaSBSb21hZ25hV2VsY29tZSIsImZvcmVDb2xvciI6IiNmZmZmZmYiLCJiYWNrQ29sb3IiOiIjZjU3YzAwIn0=.png" alt="Acquista le Experience di RomagnaWelcome" title="Acquista le Experience di RomagnaWelcome" border="0" /></a>

        <script src="https://experience.romagnawelcome.it/it/api/public"></script>
        <script>
            (function() {
                var button = new TrekkSoft.Embed.Button();
                button
                      .setAttrib("target", "fancy")
                      .setAttrib("entryPoint", "tours")
                      .setAttrib("referral", "PROMOZIONEALBERGHIERA")
                      .setAttrib("fancywidth", "615px")
                      .registerOnClick("#trekksoft_1727");
            })();
        </script>        

Per modificare la lingua del contenuto mostrato, è necessario modificare il codice lingua nello script di caricamento
.. parsed-literal::
        <script src="https://experience.romagnawelcome.it/it/api/public"></script>
sostituendo ``/it/`` con:  ``/en/``, ``/fr/`` o ``/de/``

Sarà possibile utilizzare un qualsiasi altro elemento del sito web (menù, altri pulsanti, immagini) per aprire il box, a sostituzione del puntante predefinito. E' sufficiente rimuovere dal codice precedente il pulsante preformattato, cancellando la parte
.. parsed-literal::
        <a href="#" id="trekksoft_1727"><img src="https://experience.romagnawelcome.it/cache/images/widget-buttons/eyJsYWJlbCI6Ilwvd2lkZ2V0XC9ib29rLWJ1dHRvbi5wbmciLCJjYXB0aW9uIjoiQWNxdWlzdGEgbGUgRXhwZXJpZW5jZSBkaSBSb21hZ25hV2VsY29tZSIsImZvcmVDb2xvciI6IiNmZmZmZmYiLCJiYWNrQ29sb3IiOiIjZjU3YzAwIn0=.png" alt="Acquista le Experience di RomagnaWelcome" title="Acquista le Experience di RomagnaWelcome" border="0" /></a>

ed innestrare l'ID ``id="trekksoft_1727"`` su qualunque elemento del sito web
