# DET_IoT_Telegram

<h1> Hoe bestuur je LEDS met Telegram? </h1>
Hoe je dit kan doen zal je verder in deze handleiding vinden!

<h2>Inhoudsopgave</h2>
  <li> Wat heb je nodig? </li>
  <li> Stap 1: Voorbereiding Telegram </li>
  <li> Stap 2: Telegram gebruiker ID </li>
  <li> Stap 3: Voorbereiding Arduino IDE  </li>
  <li>  </li>
  <li>  </li>
  <li>  </li>


<h2> Wat heb je nodig? </h2>
<ol>
  <li> Arduino IDE </li>
  <li> ESP8266 board </li>
  <li> Telegram op je telefoon </li>
</ol>



<h2> Stap 1: Voorbereiding Telegram </h2>
<ol>
  <li> Ga naar de appstore / google play en download Telegram. </li>
  <li> Klik op het vegrootglas rechts bovenin en zoek naar 'botfather'. </li>
  <li> Klik alsvolgt op start. </li>
  <li> Type in '/newbot'. </li>
  <li> Nu zal de botfather je vragen om de bot een naam en gebruikersnaam te geven.<br>
       Tip 1: De gebruikersnaam moet eindigen met 'bot'. Dus bijvoorbeeld BobBot of Bob_bot.<br>
       Tip 2: Ik dacht voor een simpele naam te gaan, maar nou blijkt deze gebruikersnaam al te bestaan. Zorg dat je een unieke naam kiest voor minder problemen. </li>
  <li> Als het je is gelukt om een gebruikersnaam te kiezen die nog niet is gebruikt. Dan krijg je onderstaan beeld te zien als het goed is. </li>
  <li> In het bericht wat je zojuist hebt gekregen, bewaar de token, deze ga je later nodig hebben om te kunnen interacteren met de bot!  </li> 
</ol>

<h2> Stap 2: Telegram gebruiker ID </h2>
<ol>
  <li> Iedereen kan gebruik maken van je bit, zolang die de gebruikersnaam heeft. Om ervoor te zorgen dat dit dit alleen berichten zullen worden van uw eigen telegram account, maken we een Telegram gebruikers ID aan.</li>
  <li> Ga naar je Telegram account en zoek voor 'IDBot'. En klik op start. </li>
  <li> Begin een gesprek met de bot en type '/getid'. </li>
  <li> Als het goed is heeft de IDBot je nu een gebruikers ID toegestuurd. <br>
    Belangrijk: Bewaar dit ID, deze ga je later nodig hebben!  </li>
</ol>


<h2> Stap 3: Code in Arduino IDE </h2>
<ol>
  <li> Ga naar Skech > Include Library > Manage Libraries </li>
  <li> Zoek op 'ArduinoJson' (van Benoit Blanchon) en installeer deze. <br>
        Let op: Gebruik de versie 6.15.2 van ArduinoJson.</li>
  <li> Open een nieuwe sketch, en kopieer de code van deze site: <br>
        https://raw.githubusercontent.com/RuiSantosdotme/Random-Nerd-Tutorials/master/Projects/ESP/ESP_Telegram/ESP_Telegram_Control_Outputs.ino <br>
  en plak deze in je sketch. </li>
  <li> Verander in de code je WiFi SSID en wachtwoord, maar vul ook je Bot Token en gebruikers ID in van Telegram. </li>
  <li>  </li>
  <li>  </li>
  
</ol>


<h2> Foutmeldingen: </h2>
<ol>
  <li> Dit was de eerste foutmelding die ik kreeg het moment dat ik op upload drukte. <br>
  <img width="641" alt="Scherm­afbeelding 2023-10-09 om 18 12 48" src="https://github.com/AnoukPNL/DET_IoT_Telegram/assets/112867115/ec95c547-5d6b-4adb-9787-e7ab5c458f1c"> <br>
Toen ik in opzoek ging naar wat ermee was, begon ik in de code te kijken. Hier zag ik iets over 'universal telegram bot library. Dit stond niet in de stappen, maar die heb ik gedownload. Dit leek een verbetering aangezien hij nu uploadde zonder error! Maar er gebeurde niks... </li>

   <li> Daarbij kreeg ik zo'n soort foutmelding, zie onderstaande foto. <br>
   <img width="1089" alt="Scherm­afbeelding 2023-10-09 om 20 09 55" src="https://github.com/AnoukPNL/DET_IoT_Telegram/assets/112867115/a15b7385-0f14-41d7-93d2-598f6c483656"> <br>
   Wat lijkt alsof hij de poort niet kan vinden. Daarom heb ik de applicatie opnieuw opgestart. <br>
<img width="734" alt="Scherm­afbeelding 2023-10-09 om 20 15 26" src="https://github.com/AnoukPNL/DET_IoT_Telegram/assets/112867115/6e1076c7-adb3-4a66-afce-2d99d23538eb"> <br>
Daarbij keek ik gelijk weer naar mijn poorten, en hoewel hij er wel staat als aangewezen poort, staat hij niet tussen de andere poorten. Daarom haalde ik de Arduino uit en weer in mijn laptop en uploadde ik hem weer opnieuw. Met dit keer weer een upload completed scherm, zonder foutmeldingen in het rood!

   </li>
</ol>


<h2> : </h2>
<ol>
  <li>  </li>
</ol>


<h2> Bronnenlijst: </h2>
<ol>
  <li> https://randomnerdtutorials.com/telegram-control-esp32-esp8266-nodemcu-outputs/ </li>
  <li> https://www.instructables.com/Telegram-Bot-With-ESP8266/ </li>
  <li>  </li>
</ol>
