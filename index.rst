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

Modalità fancybox
----------
La modalità fancybox consente di aprire un widget in overlay sul sito, che consente al visitatore di prenotare e concludere l'acquisto senza abbandonare il sito web dell'hotel:

.. parsed-literal::
        <a href="#" id="trekksoft_1946"><img src="https://experience.romagnawelcome.it/cache/images/widget-buttons/eyJsYWJlbCI6Ilwvd2lkZ2V0XC9ib29rLWJ1dHRvbi5wbmciLCJjYXB0aW9uIjoiUHJlbm90YSIsImZvcmVDb2xvciI6IiNmZmZmZmYiLCJiYWNrQ29sb3IiOiIjMDA4ZmJlIn0=.png" alt="Prenota" title="Prenota" border="0" /></a>
<script src="https://experience.romagnawelcome.it/it/api/public"></script>
<script>
    (function() {
        var button = new TrekkSoft.Embed.Button();
        button
              .setAttrib("target", "fancy")
              .setAttrib("entryPoint", "tours")
              .setAttrib("referral", "PROMOZIONEALBERGHIERA")
              .setAttrib("fancywidth", "615px")
              .registerOnClick("#trekksoft_1946");
    })();
</script>    


Features
--------

- Be awesome
- Make things faster

Installation
------------

Install $project by running:

    install project

Contribute
----------

- Issue Tracker: github.com/$project/$project/issues
- Source Code: github.com/$project/$project

Support
-------

If you are having issues, please let us know.
We have a mailing list located at: project@google-groups.com

License
-------

The project is licensed under the BSD license.
