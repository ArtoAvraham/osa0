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

    
