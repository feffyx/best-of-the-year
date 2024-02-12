
# Step 1
Creare un nuovo progetto Spring Boot MVC + Thymeleaf utilizzando lo Spring Initializr (potete includere anche DevTools e configurare IntelliJ come visto in classe seguendo le istruzioni allegate). <br/>
Nel progetto aggiungere un controller che risponde alla root dell’applicazione, con un metodo che restituisce una view fatta con Thymeleaf in cui viene stampato un titolo:<br/> “Best of the [anno] by [nome]” (al posto dei valori tra [] deve apparire l’anno 2023 e il vostro nome, passati come attributo attraverso il Model).
# Step 2
Aggiungere una classe che rappresenta le canzoni (Song), caratterizzata da id, titolo e autore.<br/>
Creare un altro controller dedicato alle canzoni, che risponde alla rotta “/songs”.<br/>
All’interno del controller aggiungere<br/>
un metodo privato getSongs() che restituisce una lista di oggetti di tipo Song<br/>
un metodo annotato @Getmapping che restituisce una pagina contenente l’elenco puntato con i titoli di tutte le song ottenute col metodo getSongs()<br/>
un metodo annotato @Getmapping che restituisce la pagina di dettaglio di una Song. L’id della Song da mostrare è passato dal browser come parametro della query string oppure fa parte del path della request.<br/>
# Step 3
Collegare le varie pagine con dei link:<br/>
nella home page un link che manda alla pagina con la lista delle song<br/>
nella pagina della lista delle song un link che torna alla home<br/>
ogni titolo di canzone deve essere un link che manda alla pagina di dettaglio<br/>
nella pagina di dettaglio un link che rimanda alla pagina con la lista<br/>
# BONUS:
aggiungere anche l’area con i best movies, fatta allo stesso modo di quella delle canzoni
