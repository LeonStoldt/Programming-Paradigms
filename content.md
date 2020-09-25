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
<th align="center"></th>
<th align="center">statisches Typsystem</th>
<th align="center">dynamisches Typsystem <code>Prolog</code></th>
</tr>
</thead>
<tbody>
<tr>
<td align="center"><strong>strenges Typsystem</strong></td>
<td align="center"><strong>implizites Typsystem</strong> <code>Haskell, Standard ML</code></td>
<td align="center"><strong>implizites Typsystem</strong>  <code>Lisp, Clojure, Smalltalk</code></td>
</tr>
<tr>
<td align="center"></td>
<td align="center"><strong>explizites Typsystem</strong> <code>Java</code></td>
<td align="center"><strong>explizites Typsystem</strong></td>
</tr>
<tr>
<td align="center"><strong>schwaches Typsystem</strong></td>
<td align="center"><strong>implizites Typsystem</strong></td>
<td align="center"><strong>implizites Typsystem</strong> <code>Javascript</code></td>
</tr>
<tr>
<td align="center"></td>
<td align="center"><strong>explizites Typsystem</strong> <code>C</code></td>
<td align="center"><strong>explizites Typsystem</strong></td>
</tr>
</tbody>
</table><h2 id="funktionale-programmiersprachen">Funktionale Programmiersprachen</h2>
<h3 id="clojure">Clojure</h3>
<ul>
<li>Lisp Dialekt</li>
<li>strenges, dynamisches, implizites Typsystem</li>
<li>verschiedene Programmierstile (imperativ, funktional, objektorientiert)</li>
</ul>
<h4 id="repl-read-eval-print-loop">REPL (Read-Eval-Print-Loop)</h4>
<ul>
<li>Liest den Ausdruck</li>
<li>Wertet ihn aus</li>
<li>Gibt das Ergebnis zurück</li>
</ul>
<h4 id="beispiel-code">Beispiel-Code</h4>
<pre class=" language-haskell"><code class="prism  language-haskell"><span class="token punctuation">(</span><span class="token hvariable">def</span> <span class="token builtin">filter</span> 
      <span class="token punctuation">(</span><span class="token hvariable">fn</span> <span class="token punctuation">[</span><span class="token hvariable">praed</span><span class="token operator">?</span> <span class="token hvariable">lst</span><span class="token punctuation">]</span>
        <span class="token punctuation">(</span><span class="token hvariable">cond</span> 
          <span class="token punctuation">(</span><span class="token hvariable">empty</span><span class="token operator">?</span> <span class="token hvariable">lst</span><span class="token punctuation">)</span> <span class="token punctuation">(</span><span class="token punctuation">)</span> 
          <span class="token punctuation">(</span><span class="token hvariable">praed</span><span class="token operator">?</span> <span class="token punctuation">(</span><span class="token hvariable">first</span> <span class="token hvariable">lst</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
             <span class="token punctuation">(</span><span class="token hvariable">cons</span> <span class="token punctuation">(</span><span class="token hvariable">first</span> <span class="token hvariable">lst</span><span class="token punctuation">)</span> <span class="token punctuation">(</span><span class="token builtin">filter</span> <span class="token hvariable">praed</span><span class="token operator">?</span> <span class="token punctuation">(</span><span class="token hvariable">rest</span> <span class="token hvariable">lst</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
          <span class="token operator">:</span><span class="token keyword">else</span> <span class="token punctuation">(</span><span class="token builtin">filter</span> <span class="token hvariable">praed</span><span class="token operator">?</span> <span class="token punctuation">(</span><span class="token hvariable">rest</span> <span class="token hvariable">lst</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
</code></pre>
<h3 id="standard-ml">Standard ML</h3>
<ul>
<li>funktionale Programmiersprache</li>
<li>strenges, statisches, implizites Typsystem</li>
<li>Typinferenz</li>
<li>ermöglicht Pattern-Matching</li>
</ul>
<h4 id="beispiel-code-1">Beispiel-Code:</h4>
<pre class=" language-ocaml"><code class="prism  language-ocaml"><span class="token comment">(* Filter *)</span>
<span class="token keyword">fun</span> filter <span class="token punctuation">(</span>praed<span class="token punctuation">,</span> lst<span class="token punctuation">)</span> <span class="token operator">=</span>
    <span class="token keyword">if</span> null lst
    <span class="token keyword">then</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>
    <span class="token keyword">else</span> <span class="token keyword">if</span> praed <span class="token punctuation">(</span>hd lst<span class="token punctuation">)</span>
    <span class="token keyword">then</span> 
        hd lst <span class="token punctuation">:</span><span class="token punctuation">:</span> filter <span class="token punctuation">(</span>praed<span class="token punctuation">,</span> tl lst<span class="token punctuation">)</span>
    <span class="token keyword">else</span> filter <span class="token punctuation">(</span>praed<span class="token punctuation">,</span> tl lst<span class="token punctuation">)</span>
<span class="token comment">(* Signatur von filter: fn : ('a -&gt; bool) * 'a list -&gt; 'a list *)</span>

<span class="token comment">(* Lambda Ausdruck *)</span>
fn x <span class="token operator">=&gt;</span> x<span class="token operator">+</span><span class="token number">1</span>

<span class="token comment">(* Funktion benennen *)</span>
<span class="token keyword">val</span> twice <span class="token operator">=</span> <span class="token punctuation">(</span>fn x <span class="token operator">=&gt;</span> <span class="token number">2</span><span class="token operator">*</span>x<span class="token punctuation">)</span>

<span class="token comment">(* Funktionen mit Rekursion [fun statt fn] *)</span>
<span class="token keyword">fun</span> fac n <span class="token operator">=</span> 
	<span class="token keyword">if</span> <span class="token punctuation">(</span>n<span class="token operator">=</span><span class="token number">0</span><span class="token punctuation">)</span> 
	<span class="token keyword">then</span> <span class="token number">1</span> 
	<span class="token keyword">else</span> n<span class="token operator">*</span><span class="token punctuation">(</span>fac <span class="token punctuation">(</span>n<span class="token number">-1</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

<span class="token comment">(* Funktion mit getypten Parametern *)</span>
<span class="token keyword">fun</span> pow <span class="token punctuation">(</span>x<span class="token punctuation">:</span>int<span class="token punctuation">,</span> y<span class="token punctuation">:</span>int<span class="token punctuation">)</span> <span class="token operator">=</span> 
    <span class="token keyword">if</span> y<span class="token operator">=</span><span class="token number">0</span>
    <span class="token keyword">then</span> <span class="token number">1</span>
    <span class="token keyword">else</span> x <span class="token operator">*</span> pow<span class="token punctuation">(</span>x<span class="token punctuation">,</span>y<span class="token number">-1</span><span class="token punctuation">)</span>
    
<span class="token comment">(* Tupel *)</span>
<span class="token keyword">val</span> pair <span class="token operator">=</span> <span class="token punctuation">(</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token string">"abc"</span><span class="token punctuation">)</span>

<span class="token comment">(* Liste {1} *)</span>
<span class="token number">1</span><span class="token punctuation">:</span><span class="token punctuation">:</span>nil

<span class="token comment">(* Zugriff auf das erste Listenelement *)</span>
hd list

<span class="token comment">(* Zugriff auf den Rest der Liste *)</span>
tl list

<span class="token comment">(* Records [= HashMaps] *)</span>
<span class="token keyword">val</span> car <span class="token operator">=</span> <span class="token punctuation">{</span>make <span class="token operator">=</span> <span class="token string">"Ford"</span><span class="token punctuation">,</span> built <span class="token operator">=</span> <span class="token number">1904</span><span class="token punctuation">}</span>

<span class="token comment">(* Zugriff auf HashMap-Einträge *)</span>
<span class="token directive function">#make</span> car

<span class="token comment">(* Summieren von Listpaaren *)</span>
<span class="token keyword">fun</span> sum<span class="token punctuation">_</span>pair <span class="token punctuation">(</span>a<span class="token punctuation">,</span>b<span class="token punctuation">)</span> <span class="token operator">=</span> a <span class="token operator">+</span> b<span class="token punctuation">;</span>

<span class="token keyword">fun</span> sum<span class="token punctuation">_</span>pair<span class="token punctuation">_</span>list <span class="token punctuation">(</span>lst<span class="token punctuation">)</span> <span class="token operator">=</span> 
  <span class="token keyword">if</span> <span class="token punctuation">(</span>lst <span class="token operator">=</span> nil<span class="token punctuation">)</span> 
  <span class="token keyword">then</span> <span class="token number">0</span> 
  <span class="token keyword">else</span> sum<span class="token punctuation">_</span>pair <span class="token punctuation">(</span>hd lst<span class="token punctuation">)</span> <span class="token operator">+</span> sum<span class="token punctuation">_</span>pair<span class="token punctuation">_</span>list <span class="token punctuation">(</span>tl lst<span class="token punctuation">)</span><span class="token punctuation">;</span>

sum<span class="token punctuation">_</span>pair<span class="token punctuation">_</span>list <span class="token punctuation">[</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">4</span><span class="token punctuation">,</span><span class="token number">5</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">;</span> <span class="token comment">(* =14 *)</span>

<span class="token comment">(* Extrahieren des ersten Elements von Listpaaren *)</span>
<span class="token keyword">fun</span> get<span class="token punctuation">_</span>first <span class="token punctuation">(</span>a<span class="token punctuation">,</span>b<span class="token punctuation">)</span> <span class="token operator">=</span> a<span class="token punctuation">;</span>

<span class="token keyword">fun</span> firsts <span class="token punctuation">(</span>lst<span class="token punctuation">)</span> <span class="token operator">=</span> 
  <span class="token keyword">if</span> lst <span class="token operator">=</span> nil
  <span class="token keyword">then</span> nil
  <span class="token keyword">else</span> get<span class="token punctuation">_</span>first <span class="token punctuation">(</span>hd lst<span class="token punctuation">)</span> <span class="token punctuation">:</span><span class="token punctuation">:</span> <span class="token punctuation">(</span>firsts <span class="token punctuation">(</span>tl lst<span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

firsts <span class="token punctuation">[</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">4</span><span class="token punctuation">,</span><span class="token number">5</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">;</span>

<span class="token comment">(* Datumsfunktionen (DD MM YYY) *)</span>
<span class="token keyword">fun</span> ist<span class="token punctuation">_</span>frueher <span class="token punctuation">(</span>day1 <span class="token punctuation">:</span> int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">,</span> day2 <span class="token punctuation">:</span> int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">)</span> <span class="token operator">=</span>
    <span class="token punctuation">(</span>#<span class="token number">1</span> day1<span class="token punctuation">)</span> <span class="token operator">&lt;</span> <span class="token punctuation">(</span>#<span class="token number">1</span> day2<span class="token punctuation">)</span>
    orelse <span class="token punctuation">(</span><span class="token punctuation">(</span><span class="token punctuation">(</span>#<span class="token number">2</span> day1<span class="token punctuation">)</span> <span class="token operator">&lt;</span> <span class="token punctuation">(</span>#<span class="token number">2</span> day2<span class="token punctuation">)</span><span class="token punctuation">)</span>
            andalso <span class="token punctuation">(</span><span class="token punctuation">(</span>#<span class="token number">1</span> day1<span class="token punctuation">)</span> <span class="token operator">=</span> <span class="token punctuation">(</span>#<span class="token number">1</span> day2<span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
    orelse <span class="token punctuation">(</span><span class="token punctuation">(</span><span class="token punctuation">(</span>#<span class="token number">3</span> day1<span class="token punctuation">)</span> <span class="token operator">&lt;</span> <span class="token punctuation">(</span>#<span class="token number">3</span> day2<span class="token punctuation">)</span><span class="token punctuation">)</span>
            andalso <span class="token punctuation">(</span><span class="token punctuation">(</span>#<span class="token number">2</span> day1<span class="token punctuation">)</span> <span class="token operator">=</span> <span class="token punctuation">(</span>#<span class="token number">2</span> day2<span class="token punctuation">)</span><span class="token punctuation">)</span>
            andalso <span class="token punctuation">(</span><span class="token punctuation">(</span>#<span class="token number">1</span> day1<span class="token punctuation">)</span> <span class="token operator">=</span> <span class="token punctuation">(</span>#<span class="token number">1</span> day2<span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

ist<span class="token punctuation">_</span>frueher <span class="token punctuation">(</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">4</span><span class="token punctuation">,</span><span class="token number">2017</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">7</span><span class="token punctuation">,</span><span class="token number">6</span><span class="token punctuation">,</span><span class="token number">2017</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span>datum<span class="token punctuation">:</span>int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">,</span> monat<span class="token punctuation">)</span> <span class="token operator">=</span> #<span class="token number">2</span> datum <span class="token operator">=</span> monat<span class="token punctuation">;</span>

in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2017</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span>daten<span class="token punctuation">:</span> <span class="token punctuation">(</span>int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">)</span> list<span class="token punctuation">,</span> monat <span class="token punctuation">:</span> int<span class="token punctuation">)</span> <span class="token operator">=</span> 
  <span class="token keyword">if</span> daten <span class="token operator">=</span> nil
  <span class="token keyword">then</span> nil
  <span class="token keyword">else</span> in<span class="token punctuation">_</span>monat<span class="token punctuation">(</span>hd daten<span class="token punctuation">,</span> monat<span class="token punctuation">)</span> <span class="token punctuation">:</span><span class="token punctuation">:</span> kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span>tl daten<span class="token punctuation">,</span> monat<span class="token punctuation">)</span><span class="token punctuation">;</span>

kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span><span class="token punctuation">[</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2018</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2017</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> contains <span class="token punctuation">(</span><span class="token keyword">value</span><span class="token punctuation">:</span> bool<span class="token punctuation">,</span> lst<span class="token punctuation">:</span> <span class="token punctuation">(</span>bool<span class="token punctuation">)</span> list<span class="token punctuation">)</span> <span class="token operator">=</span>
    <span class="token keyword">if</span> lst <span class="token operator">=</span> nil
    <span class="token keyword">then</span> <span class="token boolean">false</span>
    <span class="token keyword">else</span> 
      <span class="token keyword">if</span> <span class="token punctuation">(</span>hd lst<span class="token punctuation">)</span> <span class="token operator">=</span> <span class="token keyword">value</span>
      <span class="token keyword">then</span> <span class="token boolean">true</span>
      <span class="token keyword">else</span> contains <span class="token punctuation">(</span><span class="token keyword">value</span><span class="token punctuation">,</span> tl lst<span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> daten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span>daten<span class="token punctuation">:</span> <span class="token punctuation">(</span>int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">)</span> list<span class="token punctuation">,</span> monat<span class="token punctuation">:</span> int<span class="token punctuation">)</span> <span class="token operator">=</span> 
  <span class="token keyword">if</span> daten <span class="token operator">=</span> nil
  <span class="token keyword">then</span> nil
  <span class="token keyword">else</span> 
      <span class="token keyword">if</span> in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span>hd daten<span class="token punctuation">,</span> monat<span class="token punctuation">)</span>
      <span class="token keyword">then</span> <span class="token punctuation">(</span>hd daten<span class="token punctuation">)</span> <span class="token punctuation">:</span><span class="token punctuation">:</span> daten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span>tl daten<span class="token punctuation">,</span> monat<span class="token punctuation">)</span>
      <span class="token keyword">else</span> daten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span>tl daten<span class="token punctuation">,</span> monat<span class="token punctuation">)</span><span class="token punctuation">;</span>

daten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monat <span class="token punctuation">(</span><span class="token punctuation">[</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2018</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">2017</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monaten <span class="token punctuation">(</span>daten<span class="token punctuation">:</span> <span class="token punctuation">(</span>int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">)</span> list<span class="token punctuation">,</span> monate<span class="token punctuation">:</span> <span class="token punctuation">(</span>int<span class="token punctuation">)</span> list<span class="token punctuation">)</span> <span class="token operator">=</span> 
  <span class="token keyword">if</span> monate <span class="token operator">=</span> nil
  <span class="token keyword">then</span> nil
  <span class="token keyword">else</span> daten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monat<span class="token punctuation">(</span>daten<span class="token punctuation">,</span> hd monate<span class="token punctuation">)</span> <span class="token operator">@</span> kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monaten<span class="token punctuation">(</span>daten<span class="token punctuation">,</span> tl monate<span class="token punctuation">)</span><span class="token punctuation">;</span>

kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monaten <span class="token punctuation">(</span><span class="token punctuation">[</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2018</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2017</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">2018</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">2018</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">,</span> <span class="token punctuation">[</span><span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">]</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> contains<span class="token punctuation">_</span>date <span class="token punctuation">(</span>date<span class="token punctuation">:</span> int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">,</span> lst<span class="token punctuation">:</span> <span class="token punctuation">(</span>int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">)</span> list<span class="token punctuation">)</span> <span class="token operator">=</span>
    <span class="token keyword">if</span> lst <span class="token operator">=</span> nil
    <span class="token keyword">then</span> <span class="token boolean">false</span>
    <span class="token keyword">else</span> 
      <span class="token keyword">if</span> <span class="token punctuation">(</span>hd lst<span class="token punctuation">)</span> <span class="token operator">=</span> date
      <span class="token keyword">then</span> <span class="token boolean">true</span>
      <span class="token keyword">else</span> contains<span class="token punctuation">_</span>date <span class="token punctuation">(</span>date<span class="token punctuation">,</span> tl lst<span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> distinct <span class="token punctuation">(</span>daten<span class="token punctuation">:</span> <span class="token punctuation">(</span>int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">)</span> list<span class="token punctuation">)</span> <span class="token operator">=</span>
  <span class="token keyword">if</span> daten <span class="token operator">=</span> nil
  <span class="token keyword">then</span> nil
  <span class="token keyword">else</span> 
      <span class="token keyword">if</span> tl daten <span class="token operator">=</span> nil
      <span class="token keyword">then</span> <span class="token punctuation">(</span>hd daten<span class="token punctuation">)</span> <span class="token punctuation">:</span><span class="token punctuation">:</span> nil
      <span class="token keyword">else</span> 
        <span class="token keyword">if</span> contains<span class="token punctuation">_</span>date <span class="token punctuation">(</span>hd daten<span class="token punctuation">,</span> tl daten<span class="token punctuation">)</span>
        <span class="token keyword">then</span> distinct <span class="token punctuation">(</span>tl daten<span class="token punctuation">)</span>
        <span class="token keyword">else</span> <span class="token punctuation">(</span>hd daten<span class="token punctuation">)</span> <span class="token punctuation">:</span><span class="token punctuation">:</span> distinct <span class="token punctuation">(</span>tl daten<span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monaten<span class="token punctuation">_</span>2 <span class="token punctuation">(</span>daten<span class="token punctuation">:</span> <span class="token punctuation">(</span>int<span class="token operator">*</span>int<span class="token operator">*</span>int<span class="token punctuation">)</span> list<span class="token punctuation">,</span> monate<span class="token punctuation">:</span> <span class="token punctuation">(</span>int<span class="token punctuation">)</span> list<span class="token punctuation">)</span> <span class="token operator">=</span>
  distinct <span class="token punctuation">(</span>kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monaten <span class="token punctuation">(</span>daten<span class="token punctuation">,</span> monate<span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

distinct <span class="token punctuation">(</span>kalenderdaten<span class="token punctuation">_</span>in<span class="token punctuation">_</span>monaten<span class="token punctuation">_</span>2 <span class="token punctuation">(</span><span class="token punctuation">[</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2018</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2017</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">2018</span><span class="token punctuation">)</span><span class="token punctuation">,</span> <span class="token punctuation">(</span><span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">2018</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">,</span> <span class="token punctuation">[</span><span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">]</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<h1 id="ausdrucksmittel-funktionaler-programmiersprachen">3. Ausdrucksmittel funktionaler Programmiersprachen</h1>
<h2 id="pattern-matching">Pattern Matching</h2>
<h1 id="ausgewählte-kapitel">4. Ausgewählte Kapitel</h1>
<h1 id="funktionale--vs.-objektorientierte-programmierung">5. Funktionale- vs. Objektorientierte Programmierung</h1>
<h1 id="funktionale-konzepte-in-java">6. Funktionale Konzepte in Java</h1>

