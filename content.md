---


---

<h1 id="programmierparadigmen">1. Programmierparadigmen</h1>
<h3 id="was-ist-ein-programmierparadigma">Was ist ein Programmierparadigma?</h3>
<ul>
<li>Paradigma steht für Beispiel oder Vorbild</li>
<li>Kontext Programmieren: <strong>Programmierstil</strong></li>
<li>Das Erstellen von Code nach vorgegebenen Regeln</li>
</ul>
<h3 id="programmierstile">Programmierstile:</h3>

<table>
<thead>
<tr>
<th align="center">Imperative Programmierung</th>
<th align="center">Deklarative Programmierung</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center"><strong>Wie</strong> ist das Problem zu lösen?</td>
<td align="center"><strong>Was</strong> ist das zu lösende Problem?</td>
</tr>
<tr>
<td align="center">Variablen und Wertzuweisungen</td>
<td align="center">Funktionen und formale, mathematische Logik</td>
</tr>
<tr>
<td align="center">Anweisungsfolge</td>
<td align="center">Audruck, der ein Ergebnis liefert</td>
</tr>
</tbody>
</table><h4 id="zuordnung">Zuordnung:</h4>

<table>
<thead>
<tr>
<th align="center">Imperative Programmierung</th>
<th align="center">Deklarative Programmierung</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">Prozedurale Programmierung</td>
<td align="center">Funktionale Programmierung</td>
</tr>
<tr>
<td align="center">Objektorientierte Programmierung</td>
<td align="center">Logische Programmierung</td>
</tr>
</tbody>
</table><h3 id="prozedurale--vs.-objektorientierte-programmierung">Prozedurale- vs. Objektorientierte Programmierung</h3>

<table>
<thead>
<tr>
<th align="center">Prozedurale Programmierung</th>
<th align="center">Objektorientierte Programmierung</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">Denken in Prozeduren</td>
<td align="center">Daten im Mittelpunkt</td>
</tr>
<tr>
<td align="center">Für jede Unterscheidung existiert eine eigene Methode</td>
<td align="center">Objekt weiß selber, welche Antwort zu ermitteln ist</td>
</tr>
</tbody>
</table><h1 id="typsysteme">2. Typsysteme</h1>
<h2 id="datentyp">Datentyp:</h2>
<ul>
<li>Rechner arbeitet ohne Typen (nur <code>0</code> und <code>1</code>)</li>
<li>Ein Datentyp wird durch die Typisierung von Daten gebildet</li>
<li>Datentypen sind softwareseitige Konstrukte</li>
<li>Ziel: Keine Ausführung falscher Informationen auf eine Bitfolge</li>
<li>Synonym: <em>Typ</em></li>
</ul>
<h3 id="zweck-von-typisierung">Zweck von Typisierung:</h3>
<ul>
<li>Ordnung</li>
<li>Anwendung sinnloser Operationen vermeiden</li>
<li><strong>Typkompatibilität:</strong>
<ul>
<li>Anwendung eines Operators nur mit korrektem Typ möglich</li>
<li>Anwendung einer Funktion nur mit korrekten Typen möglich</li>
</ul>
</li>
</ul>

<table>
<thead>
<tr>
<th align="center">syntaktische Typkompatibilität</th>
<th align="center">semantische Typkompatibilität</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">Welche Typbezeichner und Funktionssignaturen stehen zur Verfügung?</td>
<td align="center">liefert eine Funktion das erwartete Ergebnis zurück?</td>
</tr>
<tr>
<td align="center"><strong>Vorteile:</strong> - Unterstützt modulare Entwicklung</td>
<td align="center"></td>
</tr>
<tr>
<td align="center">- Nutzung neuer Datentypen, wie vordefinierte Datentypen</td>
<td align="center"></td>
</tr>
<tr>
<td align="center"><strong>Nachteil:</strong> Syntaktisch Korrekte Implementierung kann semantisch falsch sein</td>
<td align="center"></td>
</tr>
</tbody>
</table><h2 id="typsysteme-1">Typsysteme</h2>
<p>Es gibt <strong>zwei</strong> unterschiedliche Typsysteme:</p>
<ol>
<li>
<p>Typangabe ist bei der Dekleration erforderlich:</p>
<pre class=" language-java"><code class="prism  language-java"><span class="token comment">//Beispiel in Java</span>
<span class="token keyword">int</span> i<span class="token punctuation">;</span> <span class="token comment">// Java</span>
</code></pre>
<pre class=" language-pascal"><code class="prism  language-pascal"><span class="token comment">//Beispiel in Pascal</span>
<span class="token keyword">var</span> i<span class="token punctuation">:</span> integer<span class="token punctuation">;</span>
</code></pre>
</li>
<li>
<p>Typangabe kann aus der Verwendung abgeleitet werden (<strong>Typinferenz</strong>)</p>
<pre class=" language-javascript"><code class="prism  language-javascript"><span class="token comment">//Beispiel in Clojure</span>
<span class="token punctuation">(</span>def pi <span class="token number">3.14159</span><span class="token punctuation">)</span>
</code></pre>
</li>
</ol>
<h3 id="statische-vs-dynamische-typisierung">Statische vs dynamische Typisierung</h3>

<table>
<thead>
<tr>
<th align="center">statische Typisierung</th>
<th align="center">dynamische Typisierung</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">Typprüfung erfolgt zur Übersetzungszeit</td>
<td align="center">Typprüfung folgt während der Ausführung des Programms</td>
</tr>
<tr>
<td align="center">Bsp: <code>Java, C++, C#</code></td>
<td align="center">Bsp: <code>Python, Perl, Php, Smalltalk</code></td>
</tr>
</tbody>
</table><h3 id="strenges-vs-schwaches-typsystem">Strenges vs schwaches Typsystem</h3>

<table>
<thead>
<tr>
<th align="center">strenge Typsysteme</th>
<th align="center">schwache Typsysteme</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">stellt Typensicherheit jederzeit sicher</td>
<td align="center">lässt gelegentlich auch typfremde Operationen zu</td>
</tr>
</tbody>
</table><h3 id="explizites-vs-implizites-typsystem">Explizites vs implizites Typsystem</h3>

<table>
<thead>
<tr>
<th align="center">explizite Typsysteme</th>
<th align="center">implizite Typsysteme</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">verlangt für <strong>jede</strong> Variable die Angabe eines Typs</td>
<td align="center">verlangt die Dekleration einer Variable und leitet den Typ der anderen aus der Verwendung ab</td>
</tr>
</tbody>
</table><h2 id="übersicht-typsysteme">Übersicht Typsysteme</h2>

<table>
<thead>
<tr>
<th align="center">statisches Typsystem</th>
<th align="center">dynamisches Typsystem</th>
</tr>
</thead>
<tbody></tbody>
</table><h1 id="todo---continue">TODO - continue</h1>
<h2 id="funktionale-programmiersprachen">Funktionale Programmiersprachen</h2>
<h3 id="clojure">Clojure</h3>
<h3 id="standard-ml">Standard ML</h3>
<h1 id="ausdrucksmittel-funktionaler-programmiersprachen">3. Ausdrucksmittel funktionaler Programmiersprachen</h1>
<h1 id="ausgewählte-kapitel">4. Ausgewählte Kapitel</h1>
<h1 id="funktionale--vs.-objektorientierte-programmierung">5. Funktionale- vs. Objektorientierte Programmierung</h1>
<h1 id="funktionale-konzepte-in-java">6. Funktionale Konzepte in Java</h1>

