---
created: 2024-02-11T14:00:37 (UTC +01:00)
tags: []
source: https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
author: 
---

# Grundlegende Schreib- und Formatierungssyntax - GitHub-Dokumentation

> ## Excerpt
> Erstelle mit einer einfachen Syntax eine ausgereifte Formatierung für deine Texte und Codes auf GitHub.

---
Erstelle mit einer einfachen Syntax eine ausgereifte Formatierung für deine Texte und Codes auf GitHub.

## [Überschriften](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#headings)

Um eine Überschrift zu erstellen, kannst du bis zu sechs Rautensymbole (#) vor dem Text der Überschrift hinzufügen. Die Anzahl der verwendeten Rauten (#) bestimmt die Hierarchieebene und die Schriftgröße der Überschrift.

```markdown
# A first-level heading ## A second-level heading ### A third-level heading
```

![[Markdown/attachments/headings-rendered.png]]

Wenn du mindestens zwei Überschriften verwendest, generiert GitHub automatisch ein Inhaltsverzeichnis, auf das du zugreifen kannst, indem du innerhalb des Dateiheaders auf klickst. Die einzelnen Überschriftentitel werden im Inhaltsverzeichnis aufgeführt, und du kannst auf einen Titel klicken, um zum gewünschten Abschnitt zu navigieren.

![[Markdown/attachments/headings-toc.png]]

## [Formatieren von Text](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#styling-text)

Du kannst Text in Kommentarfeldern und Dateien vom Typ `.md` mittels Fettformatierung, Kursivformatierung, durchgestrichenem, tief- oder hochgestelltem Text hervorheben.

| Style | Syntax | Tastenkombinationen | Beispiel | Output |
| --- | --- | --- | --- | --- |
| Fett | `** **` oder `__ __` | BEFEHL+B (Mac) oder STRG+B (Windows/Linux) | `**This is bold text**` | **Dieser Text ist fett.** |
| Kursiv | `* *` oder `_ _`      | BEFEHL+I (Mac) oder STRG+I (Windows/Linux) | `_This text is italicized_` | _Dieser Text ist kursiv._ |
| Durchgestrichen | `~~ ~~` | Keine | `~~This was mistaken text~~` | ~Dieser Text war falsch.~ |
| Fett und kursiv verschachtelt | `** **` und `_ _` | Keine | `**This text is _extremely_ important**` | **Dieser Text ist _sehr_ wichtig.** |
| Alles fett und kursiv | `*** ***` | Keine | `***All this text is important***` | _**Dieser gesamte Text ist wichtig.**_ |
| Tiefgestellt | `<sub> </sub>` | Keine | `This is a <sub>subscript</sub> text` | Dies ist ein <sub>tiefgestellter</sub> Text. |
| Hochgestellt | `<sup> </sup>` | Keine | `This is a <sup>superscript</sup> text` | Dies ist ein <sup>hochgestellter</sup> Text. |

## [Zitieren von Text](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#quoting-text)

Text kann mit dem folgenden Zeichen zitiert werden: \>.

```markdown
Text that is not a quote > Text that is a quote
```

Zitierter Text wird eingerückt und in einer anderen Schriftfarbe dargestellt.

![[Markdown/attachments/quoted-text-rendered.png]]

**Hinweis:** In einer Unterhaltung kannst du Text in einem Kommentar automatisch zitieren, indem du den Text markierst und anschließend R drückst. Wenn du einen vollständigen Kommentar zitieren möchtest, kannst du auf und anschließend auf **Antwort mit Zitat** klicken. Weitere Informationen zu Tastenkombinationen findest du unter [Tastenkombinationen](https://docs.github.com/de/get-started/accessibility/keyboard-shortcuts).

## [Code zitieren](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#quoting-code)

Du kannst Code oder einen Befehl innerhalb eines Satzes mit einfachen Backticks zitieren. Der Text innerhalb der Backticks wird nicht formatiert. Du kannst auch die Tastenkombination Command+E (Mac) oder STRG+E (Windows/Linux) verwenden, um die Backticks für einen Codeblock innerhalb einer Markdownzeile einzufügen.

```markdown
Use `git status` to list all new or modified files that haven't yet been committed.
```

![[Markdown/attachments/inline-code-rendered.png]]

Um Code oder einen Text in einem eigenen Absatz zu formatieren, verwende dreifache Backticks.

````
Some basic Git commands are:
```
git status
git add
git commit
```
````

![[Markdown/attachments/code-block-rendered.png]]

Weitere Informationen findest du unter [Code-Blöcke erstellen und markieren](https://docs.github.com/de/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks).

Wenn du häufig Codeausschnitte und Tabellen bearbeitest, profitierst du möglicherweise von der Aktivierung einer Schriftart mit fester Breite in allen Kommentarfeldern auf GitHub. Weitere Informationen finden Sie unter [Informationen zum Schreiben und Formatieren bei GitHub](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github#enabling-fixed-width-fonts-in-the-editor).

## [Unterstützte Farbmodelle](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#supported-color-models)

In Issues, Pull Requests und Diskussionen kannst du mit Backticks Farben innerhalb eines Satzes aufrufen. Ein unterstütztes Farbmodell in Backticks zeigt eine Visualisierung der Farbe an.

```markdown
The background color is `#ffffff` for light mode and `#000000` for dark mode.
```

![[Markdown/attachments/supported-color-models-rendered.png]]

Hier findest du die derzeit unterstützten Farbmodelle.

| Color | Syntax | Beispiel | Output |
| --- | --- | --- | --- |
| HEX | `` `#RRGGBB` `` | `` `#0969DA` `` | ![[Markdown/attachments/supported-color-models-hex-rendered.png]] |
| RGB | `` `rgb(R,G,B)` `` | `` `rgb(9, 105, 218)` `` | ![[Markdown/attachments/supported-color-models-rgb-rendered.png]] |
| HSL | `` `hsl(H,S,L)` `` | `` `hsl(212, 92%, 45%)` `` | ![[Markdown/attachments/supported-color-models-hsl-rendered.png]] |

**Hinweise:**

-   Ein unterstütztes Farbmodell darf keine führenden oder nachgestellten Leerzeichen innerhalb der Backticks aufweisen.
-   Die Visualisierung der Farbe wird nur in Issues, Pull Requests und Diskussionen unterstützt.

## [Links](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#links)

Du kannst einen Inlinelink erstellen, indem du den Text in eckige Klammern `[ ]` und die URL in runde Klammern `( )` einschließt. Du kannst auch die Tastenkombination BEFEHL+K verwenden, um einen Link zu erstellen. Wenn Text ausgewählt ist, kannst du eine URL aus der Zwischenablage einfügen, um automatisch einen Link aus der Auswahl zu erstellen.

Du kannst auch einen Markdownlink erstellen, indem du den Text markierst und die Tastenkombination BEFEHL+V verwendest. Wenn du den Text durch den Link ersetzen möchtest, verwende die Tastenkombination BEFEHL+UMSCHALT+V.

`This site was built using [GitHub Pages](https://pages.github.com/).`

![[Markdown/attachments/link-rendered.png]]

**Hinweis:** GitHub erstellt automatisch Links, wenn du gültige URLs in einen Kommentar einfügst. Weitere Informationen findest du unter [Automatisch verlinkte Verweise und URLs](https://docs.github.com/de/get-started/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls).

## [Links zu Abschnitten](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#section-links)

Du kannst direkt zu einem Abschnitt in einer gerenderten Datei verweisen, indem Du den Mauszeiger über den Abschnittstitel bewegst, um verfügbar zu machen.

![[Markdown/attachments/readme-links.png]]

## [Relative Links](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#relative-links)

Du kannst relative Links und Bildpfade in deinen gerenderten Dateien definieren, um Leser dabei zu unterstützen, in deinem Repository zu anderen Dateien zu navigieren.

Ein relativer Link ist ein Verknüpfung, die relativ zur aktuellen Datei ist. Wenn sich beispielsweise eine README-Datei im Root deines Repositorys und eine andere Datei in _docs/CONTRIBUTING.md_ befindet, sieht der relative Link zu _CONTRIBUTING.md_ in deiner README-Datei wie folgt aus:

```text
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
```

GitHub wandelt deinen relativen Link oder den Bildpfad automatisch anhand dessen um, auf welchem Branch du dich gerade befindest, damit der Link oder der Pfad immer funktioniert. Der Pfad des Links ist relativ zur aktuellen Datei. Links, die mit `/` beginnen, sind relativ zum Repositorystamm. Du kannst alle relativen Linkoperanden verwenden, z. B. `./` und `../`.

Relative Links sind für Benutzer, die dein Repository klonen, einfacher zu verwenden. Absolute Links funktionieren möglicherweise nicht in Klons deines Repositorys - wir empfehlen relative Links zu verwenden, um auf andere Dateien in deinem Repository zu verweisen.

## [Bilder](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#images)

Du kannst ein Bild anzeigen, indem du ! hinzufügst und den Alternativtext mit `[ ]` umschließt. Alternativtext ist ein kurzer Text, der den Informationen im Bild entspricht. Umschließe dann den Link für das Bild mit Klammern `()`.

`![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)`

![[Markdown/attachments/image-rendered.png]]

GitHub unterstützt das Einbetten von Bildern in Issues, Pull Requests, Diskussionen, Kommentare und Dateien vom Typ `.md`. Du kannst ein Bild aus deinem Repository anzeigen, einen Link zu einem Onlinebild hinzufügen oder ein Bild hochladen. Weitere Informationen findest du unter [Ressourcen hochladen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#uploading-assets).

**Hinweis**: Wenn du ein Bild anzeigen möchtest, das sich in deinem Repository befindet, solltest du keine absoluten Links, sondern relative Links verwenden.

Hier findest du einige Beispiele für die Verwendung relativer Links zum Anzeigen eines Bilds.

| Kontext | Relativer Link |
| --- | --- |
| In einer Datei vom Typ `.md` im gleichen Branch | `/assets/images/electrocat.png` |
| In einer Datei vom Typ `.md` in einem anderen Branch | `/../main/assets/images/electrocat.png` |
| In Issues, Pull Requests und Kommentaren des Repositorys | `../blob/main/assets/images/electrocat.png?raw=true` |
| In einer Datei vom Typ `.md` in einem anderen Repository | `/../../../../github/docs/blob/main/assets/images/electrocat.png` |
| In Issues, Pull Requests und Kommentaren eines anderen Repositorys | `../../../github/docs/blob/main/assets/images/electrocat.png?raw=true` |

**Hinweis**: Die letzten beiden relativen Links in der obigen Tabelle funktionieren nur für Bilder in einem privaten Repository, wenn der Betrachter mindestens Lesezugriff auf das private Repository besitzt, das die Bilder enthält.

Weitere Informationen findest du unter [Relative Links](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#relative-links).

### [Design angeben, in dem ein Bild angezeigt wird](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#specifying-the-theme-an-image-is-shown-to)

Du kannst das Design angeben, für das ein Bild in Markdown angezeigt wird, indem du das HTML-Element `<picture>` in Kombination mit dem Medienfeature `prefers-color-scheme` verwendest. Wir unterscheiden zwischen hellem und dunklem Farbmodus. Es sind also zwei Optionen verfügbar. Du kannst diese Optionen verwenden, um Bilder anzuzeigen, die für dunkle oder helle Hintergründe optimiert sind. Das ist besonders bei transparenten PNG-Bildern hilfreich.

Der folgende Code zeigt beispielsweise ein Bild einer Sonne für helle Designs und einen Mond für dunkle Designs an:

```html
<picture> <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png"> <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png"> <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png"> </picture>
```

Die Methode zum Angeben von Bildern basierend auf dem Design mithilfe eines Fragments, das an die URL angefügt ist (`#gh-dark-mode-only` oder `#gh-light-mode-only`), ist veraltet und wird zugunsten der oben beschriebenen neuen Methode entfernt.

## [Listen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#lists)

Du kannst eine ungeordnete Liste erstellen, indem du einer Textzeile oder mehreren Textzeilen \-, \* oder + voranstellst.

```markdown
- George Washington * John Adams + Thomas Jefferson
```

![[Markdown/attachments/unordered-list-rendered.png]]

Um deine Liste zu ordnen, stelle jeder Zeile eine Zahl voran.

```markdown
1. James Madison 2. James Monroe 3. John Quincy Adams
```

![[Markdown/attachments/ordered-list-rendered.png]]

### [Verschachtelte Listen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#nested-lists)

Du kannst eine verschachtelte Liste erstellen, indem du ein Listenelement oder mehrere Listenelemente unter einem anderen Element einrückst.

Beim Web-Editor in GitHub oder bei einem Texteditor wie [Visual Studio Code](https://code.visualstudio.com/), der eine Festbreitenschriftart verwendet, kannst du deine Liste visuell ausrichten. Gib vor dem einzurückenden Listenelement so viele Leerzeichen ein, bis das Listenzeichen (\- oder \*) direkt unter dem ersten Zeichen des darüber liegenden Elements liegt.

```markdown
1. First list item - First nested list item - Second nested list item
```

**Hinweis:** Im webbasierten Editor kannst du eine oder mehrere Textzeilen ein- oder ausrücken, indem du zuerst die gewünschten Zeilen markierst und dann TAB bzw. UMSCHALT+TAB drückst.

![[Markdown/attachments/nested-list-alignment.png]]

![[Markdown/attachments/nested-list-example-1.png]]

Um eine verschachtelte Liste im Kommentareditor auf GitHub zu erstellen, der keine nicht proportionale Schriftart verwendet, kannst du Dir das Listenelement direkt über der verschachtelten Liste ansehen und die Anzahl der Zeichen zählen, die vor dem Inhalt dieses Elements stehen. Gib diese Anzahl an Leerzeichen dann vor dem untergeordneten Listenelement ein.

In diesem Beispiel kannst du ein untergeordnetes Listenelement unter dem Listenelement `100. First list item` hinzufügen, indem du das untergeordnete Listenelement mindestens fünf Leerzeichen weit einrückst, da sich vor `First list item` fünf Zeichen (`100 .`) befinden.

```markdown
100. First list item - First nested list item
```

![[Markdown/attachments/nested-list-example-3.png]]

Du kannst mit derselben Methode mehrere Ebenen an verschachtelten Listen erstellen. Ein Beispiel: Da das erste geschachtelte Listenelement vor dem geschachtelten Listeninhalt `First nested list item` sieben Zeichen (`␣␣␣␣␣-␣`) enthält, musst du das zweite geschachtelte Listenelement um mindestens zwei weitere Zeichen (mindestens neun Leerzeichen) einrücken.

```markdown
100. First list item - First nested list item - Second nested list item
```

![[Markdown/attachments/nested-list-example-2.png]]

Weitere Beispiele findest du in der [Spezifikation zu GitHub Flavored Markdown](https://github.github.com/gfm/#example-265).

## [Aufgabenlisten](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists)

Um eine Aufgabenliste zu erstellen, stellst du den Listenelementen einen Bindestrich und ein Leerzeichen gefolgt von `[ ]` voran. Um eine Aufgabe als erledigt zu markieren, verwende `[x]`.

```markdown
- [x] #739 - [ ] https://github.com/octo-org/octo-repo/issues/740 - [ ] Add delight to the experience when all tasks are complete :tada:
```

![[Markdown/attachments/task-list-rendered-simple.png]]

Wenn die Beschreibung eines Aufgabenlistenelements mit einer Klammer beginnt, muss die Klammer mit dem Escapezeichen \\ versehen werden:

`- [ ] \(Optional) Open a followup issue`

Weitere Informationen findest du unter [Informationen zu Aufgabenlisten](https://docs.github.com/de/get-started/writing-on-github/working-with-advanced-formatting/about-task-lists).

## [Personen und Teams erwähnen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#mentioning-people-and-teams)

Du kannst eine Person oder ein [Team](https://docs.github.com/de/organizations/organizing-members-into-teams) in GitHub erwähnen, indem du @ sowie den Benutzer- oder Teamnamen eingibst. Dadurch wird eine Benachrichtigung ausgelöst und die Aufmerksamkeit auf die Unterhaltung gelenkt. Wenn du einen Kommentar bearbeitest und dabei den Benutzer- oder Teamnamen erwähnst, wird die Person respektive das Team ebenfalls benachrichtigt. Weitere Informationen zu Benachrichtigungen findest du unter [Informationen zu Benachrichtigungen](https://docs.github.com/de/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/about-notifications).

**Hinweis:** Eine Person wird nur über eine Erwähnung benachrichtigt, wenn die Person Lesezugriff auf das Repository hat. Falls das Repository einer Organisation gehört, muss die Person außerdem der Organisation angehören.

`@github/support What do you think about these updates?`

![[Markdown/attachments/mention-rendered.png]]

Wenn du ein übergeordnetes Team erwähnst, erhalten auch die Mitglieder untergeordneter Teams Benachrichtigungen, was die Kommunikation mit mehreren Personengruppen erleichtert. Weitere Informationen findest du unter [Informationen zu Teams](https://docs.github.com/de/organizations/organizing-members-into-teams/about-teams).

Wenn du das Zeichen @ eingibst, wird eine Liste der Personen oder Teams eines Projektes angezeigt. Diese Liste wird während deiner Eingabe gefiltert. Wenn du den Namen der gewünschten Person respektive des gewünschten Teams siehst, kannst du ihn mit den Pfeiltasten auswählen und die Tabulator- oder Eingabetaste drücken, um den Namen zu vervollständigen. Gib für Teams @organization/team-name ein. Daraufhin wird die Unterhaltung für alle Mitglieder des Teams abonniert.

Die automatisch vervollständigten Ergebnisse sind auf Repository-Mitarbeiter und andere Thread-Teilnehmer beschränkt.

## [Auf Issues und Pull Requests verweisen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#referencing-issues-and-pull-requests)

Du kannst eine Liste vorgeschlagener Issues und Pull Requests im Repository anzeigen, indem du # eingibst. Gib die Nummer des Issues oder Pull Requests ein, um die Liste zu filtern, und drücke dann die Tabulator- oder Eingabetaste, um das markierte Ergebnis zu vervollständigen.

Weitere Informationen findest du unter [Automatisch verlinkte Verweise und URLs](https://docs.github.com/de/get-started/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls).

## [Auf externe Ressourcen verweisen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#referencing-external-resources)

Wenn benutzerdefinierte Autolink-Referenzen für ein Repository konfiguriert sind, werden Verweise auf externe Ressourcen, beispielsweise ein JIRA-Issue oder ein Zendesk-Ticket, in verkürzte Links umgewandelt. Wenn Du wissen möchtest, welche automatische Verknüpfungen in Deinem Repository verfügbar sind, wende Dich an eine Person mit Administratorberechtigungen für das Repository. Weitere Informationen findest du unter [Automatische Verlinkungen von externen Ressourcen konfigurieren](https://docs.github.com/de/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/configuring-autolinks-to-reference-external-resources).

## [Ressourcen hochladen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#uploading-assets)

Zum Hochladen von Ressourcen (beispielsweise Bilder) kannst du Drag&Drop verwenden, die Ressourcen über einen Dateibrowser auswählen oder sie einfügen. Du kannst Ressourcen in Issues, Pull Requests, Kommentare und Dateien vom Typ `.md` in deinem Repository hochladen.

## [Emojis verwenden](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#using-emojis)

Du kannst deinem Text Emojis hinzufügen, indem du `:EMOJICODE:`, einen Doppelpunkt gefolgt vom Namen des Emojis, eingibst.

`@octocat :+1: This PR looks great - it's ready to merge! :shipit:`

![[Markdown/attachments/emoji-rendered.png]]

Wenn du : eingibst, wird eine Liste mit vorgeschlagenen Emojis angezeigt. Die Liste wird bei der Eingabe gefiltert. Wenn du das gewünschte Emoji siehst, drücke **TAB** oder die **EINGABETASTE**, um das hervorgehobene Ergebnis zu vervollständigen.

Eine vollständige Liste der verfügbaren Emojis und Codes findest du im [Spickzettel für Emojis](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md).

## [Absätze](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#paragraphs)

Um einen neuen Absatz zu erstellen, lasse eine Zeile zwischen den Textzeilen leer.

Mit der folgenden Klammersyntax kannst du deinem Inhalt Fußnoten hinzufügen:

```text
Here is a simple footnote[^1]. A footnote can also have multiple lines[^2]. [^1]: My reference. [^2]: To add line breaks within a footnote, prefix new lines with 2 spaces. This is a second line.
```

Die Fußnote wird wie folgt gerendert:

![[Markdown/attachments/footnote-rendered.png]]

**Hinweis:** Die Position einer Fußnote in deinem Markdown hat keinen Einfluss darauf, wo die Fußnote gerendert wird. Du kannst eine Fußnote direkt nach dem Verweis auf die Fußnote schreiben, und die Fußnote wird trotzdem am unteren Rand des Markdowns gerendert.

In Wikis werden Fußnoten nicht unterstützt.

## [Alerts](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#alerts)

Warnungen sind eine Markdown-Erweiterung basierend auf der Blockquote-Syntax, mit der Sie kritische Informationen hervorheben können. Auf GitHub werden sie mit charakteristischen Farben und Symbolen angezeigt, um auf die Signifikanz des Inhalts hinzuweisen.

Verwenden Sie Warnungen nur, wenn sie für den Benutzererfolg von entscheidender Bedeutung sind, und beschränken Sie sie auf ein oder zwei pro Artikel, um zu verhindern, dass der Leser überlastet wird. Darüber hinaus sollten Sie vermeiden, Benachrichtigungen nacheinander zu platzieren. Warnungen können nicht in anderen Elementen geschachtelt werden.

Um eine Warnung hinzuzufügen, verwenden Sie eine spezielle Blockquotezeile, die den Warnungstyp angibt, gefolgt von den Warnungsinformationen in einer Standardblockquote. Es stehen fünf Arten von Warnungen zur Verfügung:

```markdown
> [!NOTE] > Useful information that users should know, even when skimming content. > [!TIP] > Helpful advice for doing things better or more easily. > [!IMPORTANT] > Key information users need to know to achieve their goal. > [!WARNING] > Urgent info that needs immediate user attention to avoid problems. > [!CAUTION] > Advises about risks or negative outcomes of certain actions.
```

Hier sind die gerenderten Warnungen aufgeführt:

![[Markdown/attachments/alerts-rendered.png]]

## [Inhalt mit Kommentaren ausblenden](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#hiding-content-with-comments)

Du kannst GitHub anweisen, Inhalt aus dem gerenderten Markdown auszublenden, indem du den Inhalt in einem HTML-Kommentar platzierst.

```
&lt;!-- This content will not appear in the rendered Markdown --&gt;
```

## [Markdown-Formatierung ignorieren](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#ignoring-markdown-formatting)

Du kannst GitHub anweisen, die Markdown-Formatierung zu ignorieren (oder zu umgehen), indem du \\ vor dem Markdown-Zeichen platzierst.

`Let's rename \*our-new-project\* to \*our-old-project\*.`

![[Markdown/attachments/escaped-character-rendered.png]]

Weitere Informationen zu umgekehrten Schrägstrichen findest du in der [Markdown-Syntax](https://daringfireball.net/projects/markdown/syntax#backslash) von Daring Fireball.

**Hinweis**: Die Markdownformatierung wird im Titel eines Issues oder eines Pull Requests nicht ignoriert.

## [Deaktivieren des Markdown-Renderings](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#disabling-markdown-rendering)

Wenn du eine Markdowndatei anzeigst, kannst du oben in der Datei auf **Code** klicken, um das Rendern von Markdown zu deaktivieren und stattdessen den Quelltext der Datei anzuzeigen.

![[Markdown/attachments/display-markdown-as-source-global-nav-update.png]]

Durch das Deaktivieren des Markdownrenderings kannst du die Funktionen der Quellenansicht nutzen, wie z. B. Zeilenverknüpfungen, die beim Anzeigen von gerenderten Markdowndateien nicht verfügbar sind.

## [Weitere Informationsquellen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#further-reading)

-   [GitHub Flavored Markdown – Spezifikation](https://github.github.com/gfm/)
-   [Informationen zum Schreiben und Formatieren bei GitHub](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github)
-   [Mit erweiterter Formatierung arbeiten](https://docs.github.com/de/get-started/writing-on-github/working-with-advanced-formatting)
-   [Schnellstart zum Schreiben auf GitHub](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)
