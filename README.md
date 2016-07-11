# Arbeitszeugnis-Generator

## Projektbeschreibung
Mit dem Arbeitszeugnis-Generator erzeugen Sie schnell standardisierte Arbeitszeugnisse.
Der Vorteil im Vergleich zu einem Online-Generator ist, dass Sie Vorlagen f�r
Flie�texte sowie die Vorlage f�r das Zeugnis selbst, komplett eigenst�ndig gestalten k�nnen.

Dieses Programm ist als [Praktikantenprojekt der BROCKHAUS AG](https://blog.brockhaus-ag.de) entstanden


## Funktionen

#### :open_file_folder: Erzeugen des Zeugnisses
Die von Ihnen eingegebenen Daten zur Person und der Bewertung werden auf eine Word-Vorlage �bertragen.
Sie m�ssen die Vorlage danach nicht mehr bearbeiten, sondern k�nnen diese sofort ausdrucken.

#### :package: Nutzung eines angepassten Design-Templates
Das Zeugnis-Template k�nnen sie selbst gestalten. Das Template basiert dabei auf der Serienbrief-Funktion von Word.

#### :floppy_disk: Speichern und Laden von Zeugnissen
Die Daten der Zeugnisse werden in XML Dateien gespeichert. So k�nnen Sie Zeugnisse immer wieder Laden und z.B. als Vorlage f�r neue Zeugnisse verwenden.

#### :star: Bewertung der Arbeitsweise mit Schulnoten
Sie k�nnen f�r jede Person individuell bestimmen, in welchen Punkten (z.B. Arbeitsweise, Fachwissen usw.) Sie diese bewerten wollen.
Die Noten werden dann mithilfe von Textvorlagen in Flie�text verwandelt.  

#### :pencil2: Anpassen der Textvorlagen
Sie k�nne alle Textvorlagen zu den Bewertungskritieren, aus denen der Flie�text ensteht, selber ver�ndern.

#### :pencil: Textanpassung abh�ngig von dem Geschlecht der Person
Die Textvorlagen, sowie das Word Template, werden beim Generieren so angepasst, dass W�rter wie z.B. 'Herr' zu 'Frau' werden, wenn das
Geschlecht der Person auf weiblich gestellt wird.

| Original   | Gro�/Klein beachtet | Ausgetauscht |
| ---------- |:-------------------:| ------------ |
| Er         | :white_check_mark:  | Sie          |
| Ihm        | :white_check_mark:  | Ihr          |
| Seine      | :white_check_mark:  | Ihre         |
| Seinen     | :white_check_mark:  | Ihren        |
| Seiner     | :white_check_mark:  | Ihrer        |
| Herr       | :no_entry_sign:     | Frau         |
| Herrn      | :no_entry_sign:     | Frau         |
| Seinem     | :white_check_mark:  | Ihrem        |
| Arbeiter   | :no_entry_sign:     | Arbeiterin   |
| Praktikant | :no_entry_sign:     | Praktikantin |

##Template
Eine Standardvorlage finden Sie unter Files/Vorlage.docx. Auf diese wird zur�ckgegriffen, wenn die von Ihnen ausgew�hlte Vorlage nicht mehr zu finden ist.
Diese Vorlage k�nnen Sie benutzen oder Ver�ndern aber bitte nicht entfernen.


## Kompatibilit�t

Das Ganze ist eine Win Forms Visual Studio Solution, was bedeutet, dass es nur auf Windows ausf�hrbar ist.

Sie ben�tigen Microsoft Word um alle Features nutzen zu k�nnen.

Die Vorlagen f�r die Zeugnisse m�ssen im .docx Format vorliegen, damit das Programm diese erkennt.

##F�r Entwickler

Benutzte IDE: Visual Studio 2015

Ben�tigte Referenzen: DocumentFormat.OpenXml

```sh
PM> Install-Package DocumentFormat.OpenXml
```


##Lizenz
Diese Software unterliegt der [GNU General Public License](https://opensource.org/licenses/GPL-3.0).