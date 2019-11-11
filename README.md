# Alkuperäinen tehtävänanto

Tehtävänäsi on purkaa APIsta haettuja kryptattuja lauseita. Lauseet on kryptattu Caesar-salakirjoitusjärjestelmällä kirjaimia oikealle siirtämällä. Aakkostona toimii A-Ö. Kirjainkoolla ei ole merkitystä. Jokaisen lauseen avain on satunnainen. Käännettävissä olevat lauseet ovat suomea. Mukana on myös lauseita, jotka eivät käänny selkokieliseksi millään avaimella.

Sinun tulee luoda web-käyttöliittymä, joka näyttää lauseet jaoteltuina No bullshit ja bullshit -lauseisiin. Käännettävissä olevat no bullshit -lauseet näytetään suomeksi ja bullshit-lauseet, jotka eivät käänny selkokielisiksi, näytetään alkuperäismuodossaan.

Et saa käyttää mitään kolmannen osapuolen palvelua tai kirjastoa, joka tunnistaa kielen automaattisesti. Tekstiaineistojen, kuten sanakirjan käyttö on kuitenkin sallittua, joskin annamme lisäpisteitä ratkaisuista, jotka eivät tukeudu valmiisiin aineistoihin.

Toteutukseen käytettävät teknologiat ovat vapaasti päätettävissäsi.

Tässä ensimmäinen linkki, josta voit aloittaa: https://koodihaaste-api.solidabis.com/secret

# Toteutus

Koodi ensin pyörittää läpi viestin kerrallaan käyttäen kaikkia mahdollisia ceasar shiftauksen arvoja ja valikoi niistä parhaan sen mukaan miten siinä esiintyy suomen kielen yleisimpiä ja vähiten käytettyjä kirjaimia. Tämän jälkeen näistä pitää erotella "no bullshit" ja "bullshit" vaihtoehdot.

Aluksi koodi tutki muutamalla perussäännöillä voiko sanat olla suomea mutta äkkiä kävi ilmi, että koska joukossa on lauseita joissa osa on suomea ja osa voisi olla suomea sen mukaan missä kohtaa ja kuinka monta vokaalia/konsonanttia sanassa on, tehtävää ei voi  ratkaista täydellisesti ilman niin sanottua sanakirjaa. Tiettävästi tämä ei ole paras/tehokkain keino mutta muunlaiseen tapaan olisi ollut valmista koodia ja tehtävästä johtuen tässä on viimeiseen asti vältetty kopioimasta muualta koodia.

Koodissa on mukana sanakirja eli lähes kaikki suomen kielen sanat perusmuodossaan. Tämän lisäyksen jälkeen koodiin tuli osio joka testaa onko sana perusmuodossa sanakirjassa tai onko sana jotenkin taivutetussa muodossa. Sanalle annetaan pisteitä perustuen näihin testeihin. Koska kielessä on myös yhdyssanoja tarkistetaan jokainen sana vielä sen mukaisestikin.
