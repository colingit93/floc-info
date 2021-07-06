# FH JOANNEUM - University of Applied Sciences

## Überblick

Federated Learning of Cohorts (FLOC) ist ein neuer, heiß diskutierter Ansatz von Google um Tracking Cookies, welche hauptsächlich für kundenoptimierte Werbung verwendet werden zu ersetzten. Doch was sind Tracking Cookies, wie funktioniert FLOC, wie sieht es mit dem Datenschutz aus, gibt es Alternativen; Dies und viele weitere Fragen werden in den folgenden Kapiteln behandelt.

### (Tracking) Cookies

Beim Öffnen eine Webseite werden sogenannte Cookies im Browser des jeweiligen Nutzers gespeichert welche Nutzerbezogene Informationen in Textform enthalten. Personenbezogene Daten werden normalerweise nicht gespeichert, sollte dies dennoch der Fall sein werden diese verschlüsselt und für Dritte nicht einsehbar hinterlegt. Cookies können grundsätzlich sehr nützlich sein da sie die Nutzer Experience erhöhen indem beispielsweise der Nutzer auf der von Ihm besuchten Webseite eingeloggt bleibt, selbst dann, wenn er die Webseite schließt oder wechselt. Die in den Cookies hinterlegten Informationen können jedoch auch gewinnbringend für gezielte Werbung genutzt werden oder an Dritte weiterverkauft werden. 

Eine Sonderform von Cookies sind sogenannten Tracking-Cookies bzw. Drittanbieter-Cookies (Third-Party Cookies), welche beispielsweise von Google Ads auf Webseiten eingesetzt werden, welche mit dem Google Ads Netzwerk in Verbindung stehen. Diese Tracking-Cookies werden verwendet, um das Kaufverhalten des Nutzers Webseitenübergreifend aufzuzeichnen. In weiterer Folge kann basierend auf dem Kaufverhalten des Nutzers gezielt Werbung geschalten werden, was in weiterer Folge die Conversion Rate steigert. Diese Tracking-Cookies können sehr groß werden da Sie Webseitenübergreifend und über längere Zeit Daten sammeln; hierzu zählen beispielsweise Transaktionsverläufe, Suchanfragen, Standortdaten, Geräteinformationen, Besucherzeiten und vieles mehr. Aus diesen Daten lassen sich sehr genaue Profile eines Nutzers erstellen was aus der Sicht des Datenschutzes als sehr verwerflich angesehen wird. Die gesammelten Daten aus den Profilen können zudem an andere Unternehmen bzw. Werbeanbieter weiterverkauft werden ohne dass der Nutzer dies bemerkt. Das Hauptproblem an den Tracking Cookies ist, dass der Nutzer nicht mitbekommt, wann und welche Daten aufgezeichnet werden. Etwas entschärft wurde dies mit den GDPR Richtlinien welches für Webseiten ein sogenanntes Opt-In Verfahren vorschreibt. Dies bedeutet, dass Nutze vor der Nutzung einer Webseite explizit dem Tracking zustimmen müssen oder dies gegebenenfalls auch ablehnen können. Hier zeigte sich jedoch ein weiteres Problem nämlich, dass ein Großteil der Nutzer sich die Cookie Richtlinien nicht sorgfältig durchließt und der Einfachheit direkt auf die hervorgehobene Schaltfläche „Alle Cookies akzeptieren“ klickt um die Webseite so schnell wie möglich zu nutzen.

### Google: Nein zu Tracking Cookies

Google kündigte Anfang 2020 an, dass Tracking Cookies bis 2022 nicht mehr im eigens entwickelten Browser (Google Chrome) akzeptiert werden. Google sah sich gezwungen diese Funktion zu implementieren da anderen Browsern wie Safari oder Firefox bereits wesentlich früher Anti-Tracking Cookie Funktionen implementierten. Google Chrome ist einer der letzten Browser, welcher sich mit der Umsetzung bezüglich der Abschaffung von Tracking Cookies beschäftigt. Die Abschaffung der Tracking-Cookies ist ein Teilziel der „Privacy Sandbox“ von Google, welche den Schutz der Privatsphäre garantieren soll. Weitere Details diesbezüglich finden dich im Kapitel Datenschutz.
 https://www.cookiebot.com/de/google-third-party-cookies/
 Das Entfernen von Third Party Cookies im Chrome Browser führte zu einem Aufschrei in der Werbewelt da der Chrome Browser mit 65% den höchsten Marktanteil besitzt. Viele Werbeanbieter sind auf Tracking-Cookies angewiesen um gezielt Werbung für Nutzer zu schalten.
 https://gs.statcounter.com/browser-market-share

Doch auch Google selbst braucht Tracking Cookies denn im Jahre 2019 hatte Google einen Werbeumsatz von 134 Milliarden US-Dollar und einen Gesamtumsatz von 160 Milliarden US-Dollar. Hier zeigt sich sehr deutlich, dass für Google, Werbung eine signifikante Einnahmequelle darstellt und Tracking Cookies auch für Google von großer Bedeutung sind. Dies ist definitiv einer der Gründe, warum Google so lange gewartet hat um sich um dem Thema Tracking-Cookies anzunehmen. Je exakter das Tracking ist, desto besser kann die Werbung auf den Kunden zugeschnitten werden, was in weiterer Folge mehr Umsatz für Google bedeutet.
 https://de.statista.com/statistik/daten/studie/75188/umfrage/werbeumsatz-von-google-seit-2001/

### FLOC

Google kündigte bereits vor dem Ende der Tracking-Cookies den Nachfolger an, welcher als Federated Learning of Cohorts (FLOC) bezeichnet wird. Dieses Tracking Konzept funktioniert wird ausschließlich im Google Chrome Browser angewandt und soll verhindern, dass Webseiten nachvollziehen können auf welchen anderen Webseiten der Nutzer besucht hat. Zusätzlich sollen weit weniger Informationen den Webseiten zur Verfügung gestellt werden als über Drittanbieter-Cookies.
 Wichtig ist, Google schafft mit FLOC das Cookie-Tracking an sich nicht ab, sondern führt lediglich eine auf Privatsphäre getrimmte neue Variante des Trackings ein! Das machen Browser wie Safari und Firefox besser da diese Tracking-Cookies vollständig blockieren – im Abschnitt Alternativen wird näher auf die Implementierung anderer Browser eingegangen.

## Funktionsweise

Im Browser (Google Chrome) des jeweiligen Benutzers werden sogenannte Kohorte (Cohorts) angelegt. Der Begriff Kohort kommt aus dem Bereich der Sozialwissenschaft und bezeichnet eine Gruppe von Personen, welche ein gemeinsames Interesse besitzen. Beispielsweise befinden sich in einem Fahrzeuge-Kohort Personen, welche sich hauptsächlich für Fahrzeuge interessieren.
 https://de.wikipedia.org/wiki/Kohorte_(Sozialwissenschaft)
 In die neuen Tracking Konzept von Google werden Personen abhängig von ihrem Suchverhalten einem oder mehreren Kohorten zugeordnet.

Der entscheidende Vorteil von FLOC gegenüber Third-Party Tracking Cookies ist, dass keine detaillierten Nutzer-Profile erstellt werden, und somit wird die Privatsphäre des Nutzers geschützt. Wenn der Nutzer eine Webseite mit geschalteter Werbung besuchen, werden ihm je nachdem in welchen Kohort Gruppe(n) sich der Nutzer befindet, die entsprechende Werbung angezeigt. Die Webseite kann somit lediglich feststellen in welcher Kohort-Gruppe sich der Nutzer befindet jedoch keine weitere Profilinformationen erlangen. Wichtig anzumerken ist, dass FLOC Konzept nicht für Googles eigene Dienste wie Google Mail, Google Search, YouTube eingesetzt wird! Hier werden weiterhin Daten gesammelt, um daraus nutzerbasierte Profile zu erstellen, welche für gezielte Google Ads Werbung verwendet werden können.

Der Nutzer bekommt von der Umstellung auf FLOC nichts mit da dieser weiterhin gezielte Werbung bekommt und sich vom grundsätzlichen Verhalten des Browsers nichts ändert. In der ersten Version von FLOC sind lediglich eine geringe Anzahl von Kohorten vorgesehen und somit ist das Bild des Nutzers relativ unscharf. In späteren Versionen sollen bis zu 33.000 Kohorte möglich sein und somit ist eine sehr feine und granulare Zuordnung des Nutzers möglich was natürlich Datenschützer nicht begrüßen da dadurch möglicherweise wieder sehr genaue Profile erstellt werden können. Probleme und Datenschutzbedenken werden dafür vorgesehenen Kapitel Datenschutz & Probleme behandelt.
 https://www.eff.org/deeplinks/2021/03/google-testing-its-controversial-new-ad-targeting-tech-millions-browsers-heres

## Alternativen

Mozilla wirbt seit Jahren mit den Sicherheitsfeatures seines Browsers Firefox und ist definitiv eine alternative zu Google Chrome. Firefox blockiert bereits seit 3.September 2019 standardmäßig alle Third-Party Tracking Cookies für alle seine Nutzer. Anders als bei Google Chrome werden hier auch Tracking Cookies von Google Diensten blockiert. In der Suchleiste des Firefox Browsers befindet sich auf der linken Seite des URLs ein Schild-Symbol, welches symbolisiert, dass Cookies blockiert werden. Mit einem Klick auf das Symbol können die blockierten Tracking-Cookies angezeigt werden und falls erwünscht das Blockieren der Cookies deaktiviert werden.
 https://blog.mozilla.org/en/products/firefox/todays-firefox-blocks-third-party-tracking-cookies-and-cryptomining-by-default/

Eine besonders für Apple User interessante Alternative zu Google Chrome ist der Safari Browser welcher im März 2020 das Intelligent Tracking Prevention (ITP) Update erhalten hat. Dieses Update enthielt zahlreiche Features hinsichtlich der Privatsphäre von Nutzer. Seit diesem Update werden standardmäßig alle Third-Party Tracking Cookies im Safari Browser blockiert. Apple setzt besonders in den letzten Jahren sehr stark auf Privatsphäre und Datenschutz und hat benutzt dies auch sehr stark für Marketingzwecke.
 https://www.theverge.com/2020/3/24/21192830/apple-safari-intelligent-tracking-privacy-full-third-party-cookie-blocking

Ein Browser welcher sich ganz und gar dem Schutz der Privatsphäre seiner Nutzer verschrieben hat trägt den Namen Brave. Dieser Browser hat beispielsweise den Zugang zum Tor Netzwerk direkt integriert und zahlreiche weitere Sicherheits-Features. Wie die anderen beiden Browser blockiert auch dieser standardmäßig alle Third-Party Tracking Cookies und verhindert dadurch das Erstellen von Nutzerbasierten Profilen.
 https://brave.com/features/ https://brave.com/privacy-features/

## Datenschutz und Probleme von FLoC
Als Google seinen Plan vorstellte, Cookies von Drittanbietern durch FLoC zu ersetzen, traten eine Reihe von Datenschutzbedenken auf. Wie schon erleutert, wurde die Entscheidung im Rahmen der „Privacy Sandbox“ Initiative bekannt gegeben. Diese plant die Einführung neuer Technologien als offene Standards, um die Privatsphäre der Endnutzer zu verbessern und eine der wichtigsten Einnahmequellen von Google, gezielte Werbung, zu schützen. Nach der Vorstellung der „Privacy Sandbox“ im August 2019 gab es immer mehr Bedenken, welche Auswirkungen die im Rahmen der Initiative vorgeschlagenen neuen Tools tatsächlich auf die Privatsphäre der Nutzer haben könnten. Insbesondere die [Electronic Frontier Foundation (EFF)](https://www.eff.org/) wies in einem Artikel namens ["Don't Play in Google's Privacy Sandbox"](https://www.eff.org/deeplinks/2019/08/dont-play-googles-privacy-sandbox-1) frühzeitig auf die Gefahren die sich hinter der Privacy Sandbox und FLoC befinden hin. Einige der Hauptprobleme, die insbesondere bei FLoC identifiziert wurden sind die Vereinfachung von Fingerprinting, cross-context exposure und der Umgang des zugrunde liegende Algorithmus mit sensiblen Kategorien.

### Fingerprinting
Fingerprinting beschreibt das Sammeln von Informationen des Browsers eines Nutzers, um diesen eindeutig identifizieren zu können. Ziel ist es, gewisse Muster zu finden, welche eine Instanz eines Browsers von Millionen von anderen unterscheidet. Es gibt viele verschieden Wege und Informationen, die für die Identifikation herangezogen werden können. Das Problem bei FLoC ist, dass ein Browser jetzt nur mehr eindeutig in einem bestimmten Cohort zu identifizieren sein muss. Das wird es für Webseiten deutlich vereinfachen, einen eindeutigen Fingerprint für FLoC Nutzer zu erstellen. Google hat dieses Problem bereits bestätigt und möchte eine Lösung dafür entwickeln. Ansätze dazu gibt es bereits, allerdings befinden sich diese noch in den Kinderschuhen.

### Cross-Context Exposure
Ein weiteres Problem wird durch die Möglichkeit der Cross-Context Exposure. Diese ist dadurch gegeben, dass Webseiten die Zugriff auf personenspezifische Daten haben ebenfalls die FLoC ID des User kennen. Somit könnte die Zuordnung von Browsern und FLoC IDs an die Öffentlichkeit kommen. So könnten einerseits Informationen über die Browsinghistorie von einzelnen Benutzern nachvollzogen werden und weitere Informationen über bestimmte Cohorts bestimmt werden.

### Unbeaufsichtigter Algorithmus
Ein Punkt der für weitere Beunruhigung sorgt, ist dass der Algorithmus der Nutzer einem FLoC Cohort zuweist, keiner Kontrollinstanz unterliegt. Grundsätzlich ist der dezentrale Ansatz ohne menschliche Einsicht eher positiv, was die Privatsphäre der Nutzer betrifft. Allerdings entsteht dadurch ein weiteres Problem, nämlich stellt sich die Frage, wie der Algorithmus mit sensitiven Kategorien umgeht. Es ist nicht auszuschließen, dass der Algorithmus Personen anhand von sensiblen Merkmalen wie Geschlecht, ethnische Zugehörigkeit, Alter und Einkommen gruppiert. Um das zu verhindern, plant Google zu analysieren, [wie FLoC-Gruppen mit sensiblen Kategorien korrelieren](https://github.com/WICG/floc#excluding-sensitive-categories). Dazu würden wiederum riesige Audits anhand von Daten zu Rasse, Geschlecht, Religion, Alter, Gesundheit und finanziellem Status der Benutzer und damit wieder ein großer Eingriff in private Personenbezogenen Daten vollzogen werden.

https://www.eff.org/deeplinks/2021/03/googles-floc-terrible-idea

https://blog.mozilla.org/en/privacy-security/privacy-analysis-of-floc/

https://github.com/WICG/floc

## Motivation
Die offizielle Erklärung von Google zu ihrer „Privacy Sandbox“ Initiative ist wie folgt: 

*"Die Privacy-Sandbox-Initiative zielt darauf ab, Web-Technologien zu schaffen, die sowohl die Privatsphäre der Menschen im Internet schützen als auch Unternehmen und Entwicklern die Werkzeuge geben, um erfolgreiche digitale Unternehmen aufzubauen, damit das Internet offen und für alle zugänglich bleibt."*

Die allgemeine Auffassung ist jedoch, dass das Hauptziel darin besteht, ihre Rolle im Geschäft der gezielten Werbung zu schützen. Abgesehen von Datenschutzbedenken gibt es auch einige wettbewerbsrechtliche Bedenken bei Googles Umstellung auf FLoC. Gegenwärtig verwenden fast alle Nicht-Google-Publisher Drittanbieter-Cookies, um Nutzer zu tracken und gezielt Werbung zu schalten. Einige Unternehmen haben Bedenken geäußert, dass Google es für andere konkurrierende Online-Werbedienste schwieriger machen wird, im Ad-Tech-Sektor zu konkurrieren. Die EU hat eine [Antitrust-Untersuchung](https://ec.europa.eu/commission/presscorner/detail/en/ip_21_3143) zu diesem potenziell wettbewerbswidrigen Verhalten eingeleitet.

https://arstechnica.com/tech-policy/2021/06/eu-antitrust-regulators-launch-probe-into-googles-floc-plan/




Authors: Tom K. - Colin J.
Supervisor: Georg M.