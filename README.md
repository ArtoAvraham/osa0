# osa0
Full Stack Open

Tehtävä 0.4 Uusi Muistiinpano

SequenceDiagram 
   participant user (käyttäjä)
   participant server
   user->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    activate server
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    *käyttäjä avaa sivun selaimessa*
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    *käyttäjä lisää kommentin: "Ohjelmointi on hauskaa"*
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    *Käyttäjä tallentaa kommentin valitsemalla tallenna / commit changes*
      user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
      *serveri rekisteröi kommentin ja tulostaa kommentin "Ohjelmointi on hauskaa"*
      *nyt kommentti näkyy selaimen sivussa: https://studies.cs.helsinki.fi/exampleapp/notes*

      Tehtävä 0,5 Single page app

SequenceDiagram 
   participant user (käyttäjä)
   participant server
   user->>server: GET https://studies.cs.helsinki.fi/exampleapp/html
    activate server
    HTML Document
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    CSS Document
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    Javascript file 
    <form id="notes_form">
    <input type="text" name "note">
    <br>
    <input type="submit" value "save">
    </form>
    *single page apissa Javascript tiedosto latautuu spa muotoon* 
    *form tagi määrittyy eri tavalla*

    Tehtävä 0.6 Uusi Muistiinpano

    SequenceDiagram 
   participant user (käyttäjä)
   participant server
   user->>server: GET https://studies.cs.helsinki.fi/exampleapp/html
    activate server
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/css
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    *käyttäjä avaa single app sivun selaimessa*
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    *käyttäjä lisää kommentin: "Ohjelmointi on hauskaa"*
    user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    *Käyttäjä tallentaa kommentin valitsemalla tallenna / commit changes*
      user -->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
      *serveri rekisteröi kommentin ja tulostaa kommentin "Ohjelmointi on hauskaa"*
      *nyt kommentti näkyy selaimen sivussa: https://studies.cs.helsinki.fi/exampleapp/spa.js*
    
    
    
