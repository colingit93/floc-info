# FH JOANNEUM - University of Applied Sciences

## Überblick :page_with_curl:

Federated Learning of Cohorts (FLOC) ist ein neuer, heiß diskutierter Ansatz von Google um Tracking Cookies, welche hauptsächlich für kundenoptimierte Werbung verwendet werden zu ersetzten. Doch was sind Tracking Cookies, wie funktioniert FLOC, wie sieht es mit dem Datenschutz aus, gibt es Alternativen; Dies und viele weitere Fragen werden in den folgenden Kapiteln behandelt.

### (Tracking) Cookies :cookie:

Beim Öffnen eine Webseite werden sogenannte Cookies im Browser des jeweiligen Nutzers gespeichert welche Nutzerbezogene Informationen in Textform enthalten. Personenbezogene Daten werden normalerweise nicht gespeichert, sollte dies dennoch der Fall sein werden diese verschlüsselt und für Dritte nicht einsehbar hinterlegt. Cookies können grundsätzlich sehr nützlich sein da sie die Nutzer Experience erhöhen indem beispielsweise der Nutzer auf der von Ihm besuchten Webseite eingeloggt bleibt, selbst dann, wenn er die Webseite schließt oder wechselt. Die in den Cookies hinterlegten Informationen können jedoch auch gewinnbringend für gezielte Werbung genutzt werden oder an Dritte weiterverkauft werden. [IONOS, Was-sind-cookies, 2020](https://www.ionos.at/digitalguide/hosting/hosting-technik/was-sind-cookies/)

Eine Sonderform von Cookies sind sogenannten Tracking-Cookies bzw. Drittanbieter-Cookies (Third-Party Cookies), welche beispielsweise von Google Ads auf Webseiten eingesetzt werden, welche mit dem Google Ads Netzwerk in Verbindung stehen. Diese Tracking-Cookies werden verwendet, um das Kaufverhalten des Nutzers Webseitenübergreifend aufzuzeichnen. In weiterer Folge kann basierend auf dem Kaufverhalten des Nutzers gezielt Werbung geschalten werden, was in weiterer Folge die Conversion Rate steigert. Diese Tracking-Cookies können sehr groß werden da Sie Webseitenübergreifend und über längere Zeit Daten sammeln; hierzu zählen beispielsweise Transaktionsverläufe, Suchanfragen, Standortdaten, Geräteinformationen, Besucherzeiten und vieles mehr. Aus diesen Daten lassen sich sehr genaue Profile eines Nutzers erstellen was aus der Sicht des Datenschutzes als sehr verwerflich angesehen wird. Die gesammelten Daten aus den Profilen können zudem an andere Unternehmen bzw. Werbeanbieter weiterverkauft werden ohne dass der Nutzer dies bemerkt. Das Hauptproblem an den Tracking Cookies ist, dass der Nutzer nicht mitbekommt, wann und welche Daten aufgezeichnet werden. Etwas entschärft wurde dies mit den GDPR Richtlinien welches für Webseiten ein sogenanntes Opt-In Verfahren vorschreibt. Dies bedeutet, dass Nutze vor der Nutzung einer Webseite explizit dem Tracking zustimmen müssen oder dies gegebenenfalls auch ablehnen können. Hier zeigte sich jedoch ein weiteres Problem nämlich, dass ein Großteil der Nutzer sich die Cookie Richtlinien nicht sorgfältig durchließt und der Einfachheit direkt auf die hervorgehobene Schaltfläche „Alle Cookies akzeptieren“ klickt um die Webseite so schnell wie möglich zu nutzen. [Cookiebot, Tracking-Cookies und die DSGVO, 2020](https://www.cookiebot.com/de/tracking-cookies-dsgvo/)

### Google: "Nein zu Tracking Cookies" :no_entry:

Google kündigte Anfang 2020 an, dass Tracking Cookies bis 2022 nicht mehr im eigens entwickelten Browser (Google Chrome) akzeptiert werden. Google sah sich gezwungen diese Funktion zu implementieren da anderen Browsern wie Safari oder Firefox bereits wesentlich früher Anti-Tracking Cookie Funktionen implementierten. Google Chrome ist einer der letzten Browser, welcher sich mit der Umsetzung bezüglich der Abschaffung von Tracking Cookies beschäftigt. Die Abschaffung der Tracking-Cookies ist ein Teilziel der „Privacy Sandbox“ von Google, welche den Schutz der Privatsphäre garantieren soll. Weitere Details diesbezüglich finden dich im Kapitel Datenschutz. [Cookiebot, Google beendet Nutzung von Third Party-Cookies in Chrome](https://www.cookiebot.com/de/google-third-party-cookies/)
 Das Entfernen von Third Party Cookies im Chrome Browser führte zu einem Aufschrei in der Werbewelt da der Chrome Browser mit 65% den höchsten Marktanteil besitzt. Viele Werbeanbieter sind auf Tracking-Cookies angewiesen um gezielt Werbung für Nutzer zu schalten.
 https://gs.statcounter.com/browser-market-share

Doch auch Google selbst braucht Tracking Cookies denn im Jahre 2019 hatte Google einen Werbeumsatz von 134 Milliarden US-Dollar und einen Gesamtumsatz von 160 Milliarden US-Dollar. Hier zeigt sich sehr deutlich, dass für Google, Werbung eine signifikante Einnahmequelle darstellt und Tracking Cookies auch für Google von großer Bedeutung sind. Dies ist definitiv einer der Gründe, warum Google so lange gewartet hat um sich um dem Thema Tracking-Cookies anzunehmen. Je exakter das Tracking ist, desto besser kann die Werbung auf den Kunden zugeschnitten werden, was in weiterer Folge mehr Umsatz für Google bedeutet.
 https://de.statista.com/statistik/daten/studie/75188/umfrage/werbeumsatz-von-google-seit-2001/

### FLOC :package:

Google kündigte bereits vor dem Ende der Tracking-Cookies den Nachfolger an, welcher als Federated Learning of Cohorts (FLOC) bezeichnet wird. Dieses Tracking Konzept funktioniert wird ausschließlich im Google Chrome Browser angewandt und soll verhindern, dass Webseiten nachvollziehen können auf welchen anderen Webseiten der Nutzer besucht hat. Zusätzlich sollen weit weniger Informationen den Webseiten zur Verfügung gestellt werden als über Drittanbieter-Cookies.
Wichtig ist, Google schafft mit FLOC das Cookie-Tracking an sich nicht ab, sondern führt lediglich eine auf Privatsphäre getrimmte neue Variante des Trackings ein! Das machen Browser wie Safari und Firefox besser da diese Tracking-Cookies vollständig blockieren – im Abschnitt Alternativen wird näher auf die Implementierung anderer Browser eingegangen.

## Funktionsweise :microscope:

Im Browser (Google Chrome) des jeweiligen Benutzers werden sogenannte Kohorte (Cohorts) angelegt. Der Begriff Kohort kommt aus dem Bereich der Sozialwissenschaft und bezeichnet eine Gruppe von Personen, welche ein gemeinsames Interesse besitzen. Beispielsweise befinden sich in einem Fahrzeuge-Kohort Personen, welche sich hauptsächlich für Fahrzeuge interessieren.
 https://de.wikipedia.org/wiki/Kohorte_(Sozialwissenschaft)
In die neuen Tracking Konzept von Google werden Personen abhängig von ihrem Suchverhalten einem oder mehreren Kohorten zugeordnet.

Der entscheidende Vorteil von FLOC gegenüber Third-Party Tracking Cookies ist, dass keine detaillierten Nutzer-Profile erstellt werden, und somit wird die Privatsphäre des Nutzers geschützt. Wenn der Nutzer eine Webseite mit geschalteter Werbung besuchen, werden ihm je nachdem in welchen Kohort Gruppe(n) sich der Nutzer befindet, die entsprechende Werbung angezeigt. Die Webseite kann somit lediglich feststellen in welcher Kohort-Gruppe sich der Nutzer befindet jedoch keine weitere Profilinformationen erlangen. Wichtig anzumerken ist, dass FLOC Konzept nicht für Googles eigene Dienste wie Google Mail, Google Search, YouTube eingesetzt wird! Hier werden weiterhin Daten gesammelt, um daraus nutzerbasierte Profile zu erstellen, welche für gezielte Google Ads Werbung verwendet werden können.

Der Nutzer bekommt von der Umstellung auf FLOC nichts mit da dieser weiterhin gezielte Werbung bekommt und sich vom grundsätzlichen Verhalten des Browsers nichts ändert. In der ersten Version von FLOC sind lediglich eine geringe Anzahl von Kohorten vorgesehen und somit ist das Bild des Nutzers relativ unscharf. In späteren Versionen sollen bis zu 33.000 Kohorte möglich sein und somit ist eine sehr feine und granulare Zuordnung des Nutzers möglich was natürlich Datenschützer nicht begrüßen da dadurch möglicherweise wieder sehr genaue Profile erstellt werden können. Probleme und Datenschutzbedenken werden dafür vorgesehenen Kapitel Datenschutz & Probleme behandelt.
 https://www.eff.org/deeplinks/2021/03/google-testing-its-controversial-new-ad-targeting-tech-millions-browsers-heres

## Alternativen :zap:

Mozilla wirbt seit Jahren mit den Sicherheitsfeatures seines Browsers Firefox und ist definitiv eine alternative zu Google Chrome. Firefox blockiert bereits seit 3.September 2019 standardmäßig alle Third-Party Tracking Cookies für alle seine Nutzer. Anders als bei Google Chrome werden hier auch Tracking Cookies von Google Diensten blockiert. In der Suchleiste des Firefox Browsers befindet sich auf der linken Seite des URLs ein Schild-Symbol, welches symbolisiert, dass Cookies blockiert werden. Mit einem Klick auf das Symbol können die blockierten Tracking-Cookies angezeigt werden und falls erwünscht das Blockieren der Cookies deaktiviert werden. [Marissa Wood, 3.09.2019](https://blog.mozilla.org/en/products/firefox/todays-firefox-blocks-third-party-tracking-cookies-and-cryptomining-by-default/)

Eine besonders für Apple User interessante Alternative zu Google Chrome ist der Safari Browser welcher im März 2020 das Intelligent Tracking Prevention (ITP) Update erhalten hat. Dieses Update enthielt zahlreiche Features hinsichtlich der Privatsphäre von Nutzer. Seit diesem Update werden standardmäßig alle Third-Party Tracking Cookies im Safari Browser blockiert. Apple setzt besonders in den letzten Jahren sehr stark auf Privatsphäre und Datenschutz und hat benutzt dies auch sehr stark für Marketingzwecke.
 https://www.theverge.com/2020/3/24/21192830/apple-safari-intelligent-tracking-privacy-full-third-party-cookie-blocking

Ein Browser welcher sich ganz und gar dem Schutz der Privatsphäre seiner Nutzer verschrieben hat trägt den Namen Brave. Dieser Browser hat beispielsweise den Zugang zum Tor Netzwerk direkt integriert und zahlreiche weitere Sicherheits-Features. Wie die anderen beiden Browser blockiert auch dieser standardmäßig alle Third-Party Tracking Cookies und verhindert dadurch das Erstellen von Nutzerbasierten Profilen.
 https://brave.com/features/ https://brave.com/privacy-features/





Authors: Tom K. - Colin J.
Supervisor: Georg M.
Version: 0.1