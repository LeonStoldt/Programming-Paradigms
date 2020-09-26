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
<h2 id="datentypen">Datentypen</h2>
<p>Erstellung neuer Datentypen in SML:</p>
<pre class=" language-ocaml"><code class="prism  language-ocaml">datatype shape <span class="token operator">=</span>
         Rectangle <span class="token keyword">of</span> real <span class="token operator">*</span> real
         <span class="token operator">|</span> Circle <span class="token keyword">of</span> real
</code></pre>
<h2 id="pattern-matching">Pattern Matching</h2>
<ul>
<li>Unterscheidung von Typen durch <code>muster =&gt; ausdruck</code></li>
<li>Verschiedene Zweige werden durch <code>|</code> getrennt</li>
</ul>
<pre class=" language-ocaml"><code class="prism  language-ocaml"><span class="token keyword">fun</span> shape<span class="token punctuation">_</span>area s <span class="token operator">=</span>
    case s <span class="token keyword">of</span>
        Rectangle<span class="token punctuation">(</span>w<span class="token punctuation">,</span> h<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> w <span class="token operator">*</span> h
      <span class="token operator">|</span> Circle<span class="token punctuation">(</span>r<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token number">3.14159</span> <span class="token operator">*</span> r <span class="token operator">*</span> r
</code></pre>
<h3 id="verwendung-von-pattern-matching">Verwendung von Pattern Matching</h3>
<h4 id="beispiel-code-2">Beispiel-Code:</h4>
<pre class=" language-ocaml"><code class="prism  language-ocaml"><span class="token keyword">fun</span> sum<span class="token punctuation">_</span>list <span class="token punctuation">(</span>xs <span class="token punctuation">:</span> int list<span class="token punctuation">)</span> <span class="token operator">=</span>
	<span class="token keyword">if</span> xs <span class="token operator">=</span> nil
	<span class="token keyword">then</span> <span class="token number">0</span>
	<span class="token keyword">else</span> hd<span class="token punctuation">(</span>xs<span class="token punctuation">)</span> <span class="token operator">+</span> sum<span class="token punctuation">_</span>list<span class="token punctuation">(</span>tl xs<span class="token punctuation">)</span>
    
<span class="token keyword">fun</span> sum<span class="token punctuation">_</span>list xs <span class="token operator">=</span>
	case xs <span class="token keyword">of</span>
		<span class="token punctuation">[</span><span class="token punctuation">]</span> <span class="token operator">=&gt;</span> <span class="token number">0</span>
		<span class="token operator">|</span> x<span class="token punctuation">:</span><span class="token punctuation">:</span>xs’ <span class="token operator">=&gt;</span> x <span class="token operator">+</span> sum<span class="token punctuation">_</span>list xs’

datatype exp <span class="token operator">=</span> Constant <span class="token keyword">of</span> int
                <span class="token operator">|</span> Negate <span class="token keyword">of</span> exp
                <span class="token operator">|</span> Add <span class="token keyword">of</span> exp <span class="token operator">*</span> exp
                <span class="token operator">|</span> Multiply <span class="token keyword">of</span> exp <span class="token operator">*</span> exp<span class="token punctuation">;</span>

<span class="token keyword">fun</span> eval exp <span class="token operator">=</span> 
  case exp <span class="token keyword">of</span>
    Constant<span class="token punctuation">(</span>i<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> i
  <span class="token operator">|</span> Negate<span class="token punctuation">(</span>ex<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token operator">~</span><span class="token punctuation">(</span>eval<span class="token punctuation">(</span>ex<span class="token punctuation">)</span><span class="token punctuation">)</span>
  <span class="token operator">|</span> Add<span class="token punctuation">(</span>sum1<span class="token punctuation">,</span> sum2<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> eval<span class="token punctuation">(</span>sum1<span class="token punctuation">)</span> <span class="token operator">+</span> eval<span class="token punctuation">(</span>sum2<span class="token punctuation">)</span>
  <span class="token operator">|</span> Multiply<span class="token punctuation">(</span>fac1<span class="token punctuation">,</span> fac2<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> eval<span class="token punctuation">(</span>fac1<span class="token punctuation">)</span> <span class="token operator">*</span> eval<span class="token punctuation">(</span>fac2<span class="token punctuation">)</span><span class="token punctuation">;</span>

eval <span class="token punctuation">(</span>Add <span class="token punctuation">(</span>Constant <span class="token number">19</span><span class="token punctuation">,</span> Negate <span class="token punctuation">(</span>Constant <span class="token number">4</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> list<span class="token punctuation">_</span>of<span class="token punctuation">_</span>constants <span class="token punctuation">(</span>lst<span class="token punctuation">:</span> exp list<span class="token punctuation">)</span> <span class="token operator">=</span>
  <span class="token keyword">if</span> lst <span class="token operator">=</span> nil
  <span class="token keyword">then</span> nil
  <span class="token keyword">else</span>
    case hd lst <span class="token keyword">of</span>
      Constant<span class="token punctuation">(</span>i<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> i <span class="token punctuation">:</span><span class="token punctuation">:</span> list<span class="token punctuation">_</span>of<span class="token punctuation">_</span>constants<span class="token punctuation">(</span>tl lst<span class="token punctuation">)</span>
    <span class="token operator">|</span> <span class="token punctuation">_</span> <span class="token operator">=&gt;</span> list<span class="token punctuation">_</span>of<span class="token punctuation">_</span>constants<span class="token punctuation">(</span>tl lst<span class="token punctuation">)</span><span class="token punctuation">;</span>

list<span class="token punctuation">_</span>of<span class="token punctuation">_</span>constants <span class="token punctuation">[</span><span class="token punctuation">(</span>Add <span class="token punctuation">(</span>Constant <span class="token number">19</span><span class="token punctuation">,</span> Negate <span class="token punctuation">(</span>Constant <span class="token number">4</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">,</span> Constant <span class="token number">19</span><span class="token punctuation">,</span> <span class="token punctuation">(</span>Constant <span class="token number">5</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> get<span class="token punctuation">_</span>bigger <span class="token punctuation">(</span>a<span class="token punctuation">:</span>int<span class="token punctuation">,</span> b<span class="token punctuation">:</span>int<span class="token punctuation">)</span> <span class="token operator">=</span>
  <span class="token keyword">if</span> a <span class="token operator">&gt;</span> b
  <span class="token keyword">then</span> a
  <span class="token keyword">else</span> b<span class="token punctuation">;</span>

<span class="token keyword">fun</span> largest<span class="token punctuation">_</span>constant<span class="token punctuation">_</span>helper<span class="token punctuation">(</span>lst<span class="token punctuation">:</span> int list<span class="token punctuation">)</span> <span class="token operator">=</span>
case lst <span class="token keyword">of</span>
  <span class="token punctuation">[</span><span class="token punctuation">]</span> <span class="token operator">=&gt;</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>
  <span class="token operator">|</span> c<span class="token punctuation">:</span><span class="token punctuation">:</span><span class="token punctuation">[</span><span class="token punctuation">]</span> <span class="token operator">=&gt;</span> <span class="token punctuation">[</span>c<span class="token punctuation">]</span>
  <span class="token operator">|</span> c<span class="token punctuation">:</span><span class="token punctuation">:</span>c2<span class="token punctuation">:</span><span class="token punctuation">:</span>cs' <span class="token operator">=&gt;</span> largest<span class="token punctuation">_</span>constant<span class="token punctuation">_</span>helper <span class="token punctuation">(</span>get<span class="token punctuation">_</span>bigger<span class="token punctuation">(</span>c<span class="token punctuation">,</span> c2<span class="token punctuation">)</span> <span class="token punctuation">:</span><span class="token punctuation">:</span> cs'<span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> largest<span class="token punctuation">_</span>constant<span class="token punctuation">(</span>lst<span class="token punctuation">:</span> exp list<span class="token punctuation">)</span> <span class="token operator">=</span> largest<span class="token punctuation">_</span>constant<span class="token punctuation">_</span>helper<span class="token punctuation">(</span>list<span class="token punctuation">_</span>of<span class="token punctuation">_</span>constants<span class="token punctuation">(</span>lst<span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

largest<span class="token punctuation">_</span>constant <span class="token punctuation">[</span><span class="token punctuation">(</span>Add <span class="token punctuation">(</span>Constant <span class="token number">19</span><span class="token punctuation">,</span> Negate <span class="token punctuation">(</span>Constant <span class="token number">4</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">,</span> Constant <span class="token number">19</span><span class="token punctuation">,</span> <span class="token punctuation">(</span>Constant <span class="token number">5</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">;</span>

<span class="token keyword">fun</span> number<span class="token punctuation">_</span>of<span class="token punctuation">_</span>adds <span class="token punctuation">(</span>lst<span class="token punctuation">:</span> exp list<span class="token punctuation">)</span> <span class="token operator">=</span>
  <span class="token keyword">if</span> lst <span class="token operator">=</span> nil
  <span class="token keyword">then</span> <span class="token number">0</span>
  <span class="token keyword">else</span>
    case hd lst <span class="token keyword">of</span>
      Add<span class="token punctuation">(</span>a<span class="token punctuation">,</span>b<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token number">1</span> <span class="token operator">+</span> number<span class="token punctuation">_</span>of<span class="token punctuation">_</span>adds<span class="token punctuation">(</span>tl lst<span class="token punctuation">)</span>
    <span class="token operator">|</span> <span class="token punctuation">_</span> <span class="token operator">=&gt;</span> <span class="token number">0</span> <span class="token operator">+</span> number<span class="token punctuation">_</span>of<span class="token punctuation">_</span>adds<span class="token punctuation">(</span>tl lst<span class="token punctuation">)</span><span class="token punctuation">;</span>

number<span class="token punctuation">_</span>of<span class="token punctuation">_</span>adds <span class="token punctuation">[</span><span class="token punctuation">(</span>Add <span class="token punctuation">(</span>Constant <span class="token number">19</span><span class="token punctuation">,</span> Negate <span class="token punctuation">(</span>Constant <span class="token number">4</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">,</span> Constant <span class="token number">19</span><span class="token punctuation">,</span> Constant <span class="token number">5</span><span class="token punctuation">,</span> <span class="token punctuation">(</span>Add <span class="token punctuation">(</span>Constant <span class="token number">19</span><span class="token punctuation">,</span> Negate <span class="token punctuation">(</span>Constant <span class="token number">4</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
</code></pre>
<h2 id="curryfizierung---partielle-anwendung">Curryfizierung - partielle Anwendung</h2>
<pre class=" language-ocaml"><code class="prism  language-ocaml"><span class="token comment">(* Bisherige Form von mehreren Parametern *)</span>
<span class="token keyword">fun</span> sorted3<span class="token punctuation">_</span>tupled <span class="token punctuation">(</span>x<span class="token punctuation">,</span>y<span class="token punctuation">,</span>z<span class="token punctuation">)</span> <span class="token operator">=</span> z <span class="token operator">&gt;=</span> y andalso y <span class="token operator">&gt;=</span> x

<span class="token comment">(* Curryfizierte Funktion *)</span>
<span class="token keyword">fun</span> sorted3 x y z <span class="token operator">=</span> z <span class="token operator">&gt;=</span> y andalso y <span class="token operator">&gt;=</span> x
</code></pre>
<h4 id="partielle-anwendung">Partielle Anwendung:</h4>
<ul>
<li>Aufruf der Funktion mit weniger Argumenten (hier &lt; 3)</li>
<li>wird häufig für Funktionen höherer Ordnung verwendet</li>
</ul>
<pre class=" language-ocaml"><code class="prism  language-ocaml"><span class="token comment">(* Funktionen höherer Ordnung *)</span>
<span class="token keyword">val</span> List<span class="token punctuation">.</span>map <span class="token operator">=</span> fn <span class="token punctuation">:</span> <span class="token punctuation">(</span>’a <span class="token operator">-&gt;</span> ’b<span class="token punctuation">)</span> <span class="token operator">-&gt;</span> ’a list <span class="token operator">-&gt;</span> ’b list

<span class="token keyword">val</span> List<span class="token punctuation">.</span>filter <span class="token operator">=</span> fn <span class="token punctuation">:</span> <span class="token punctuation">(</span>’a <span class="token operator">-&gt;</span> bool<span class="token punctuation">)</span> <span class="token operator">-&gt;</span> ’a list <span class="token operator">-&gt;</span> ’a list

<span class="token keyword">val</span> List<span class="token punctuation">.</span>foldl <span class="token operator">=</span> fn <span class="token punctuation">:</span> <span class="token punctuation">(</span>’a <span class="token operator">*</span> ’b <span class="token operator">-&gt;</span> ’b<span class="token punctuation">)</span> <span class="token operator">-&gt;</span> ’b <span class="token operator">-&gt;</span> ’a list <span class="token operator">-&gt;</span> ’b
</code></pre>
<h2 id="clojure-1">Clojure</h2>
<ul>
<li>Im Gegensatz zu SML: dynamisch getypte Sprache</li>
<li>Prefixnotation</li>
<li>Verwendung der JVM (wird zu bytecode compiliert)</li>
</ul>
<h4 id="grundlagen">Grundlagen:</h4>
<pre class=" language-typescript"><code class="prism  language-typescript"><span class="token comment">// list</span>
'<span class="token punctuation">(</span><span class="token number">1</span>  <span class="token number">2</span>  <span class="token number">3</span><span class="token punctuation">)</span>
<span class="token comment">// vector</span>
<span class="token punctuation">[</span><span class="token number">1</span>  <span class="token number">2</span>  <span class="token number">3</span><span class="token punctuation">]</span>
<span class="token comment">// set</span>
#<span class="token punctuation">{</span><span class="token number">1</span>  <span class="token number">2</span>  <span class="token number">3</span><span class="token punctuation">}</span>
<span class="token comment">// map</span>
<span class="token punctuation">{</span><span class="token punctuation">:</span>a  <span class="token number">1</span><span class="token punctuation">,</span> <span class="token punctuation">:</span>b  <span class="token number">2</span><span class="token punctuation">}</span>

<span class="token comment">// Function</span>
<span class="token punctuation">(</span>defn  greet <span class="token punctuation">[</span>name<span class="token punctuation">]</span> <span class="token punctuation">(</span>str  <span class="token string">"Hello, "</span> name<span class="token punctuation">)</span> <span class="token punctuation">)</span>

<span class="token comment">// Bedingungen</span>
<span class="token punctuation">(</span><span class="token keyword">if</span> <span class="token punctuation">(</span>even<span class="token operator">?</span>  <span class="token number">2</span><span class="token punctuation">)</span>
	<span class="token string">"even"</span>
	<span class="token string">"odd"</span><span class="token punctuation">)</span>


<span class="token punctuation">(</span><span class="token function">cond</span> 
	<span class="token punctuation">(</span><span class="token operator">&lt;</span> x <span class="token number">2</span><span class="token punctuation">)</span> <span class="token string">"Case 1"</span>
	<span class="token punctuation">(</span><span class="token operator">&lt;</span> x <span class="token number">10</span><span class="token punctuation">)</span> <span class="token string">"Case 2"</span>
	<span class="token punctuation">:</span><span class="token keyword">else</span>  <span class="token string">"Case 3"</span><span class="token punctuation">)</span>

<span class="token comment">// Zugriff auf eine Liste</span>
<span class="token punctuation">(</span><span class="token function">first</span> <span class="token punctuation">(</span>cons a list<span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token operator">=</span> <span class="token function">a</span>
<span class="token punctuation">(</span><span class="token function">rest</span> <span class="token punctuation">(</span>cons a list<span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token operator">=</span> list
</code></pre>
<h4 id="beispiel-code-3">Beispiel-Code:</h4>
<pre class=" language-python"><code class="prism  language-python"><span class="token punctuation">(</span><span class="token keyword">def</span> make<span class="token operator">-</span>add
	<span class="token punctuation">(</span>fn <span class="token punctuation">[</span>a<span class="token punctuation">]</span>
		<span class="token punctuation">(</span>fn <span class="token punctuation">[</span>b<span class="token punctuation">]</span>
			<span class="token punctuation">(</span><span class="token operator">+</span> a b<span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

<span class="token punctuation">(</span><span class="token keyword">def</span> make<span class="token operator">-</span>prepend
  <span class="token punctuation">(</span>fn <span class="token punctuation">[</span>a<span class="token punctuation">]</span>
    <span class="token punctuation">(</span>fn <span class="token punctuation">[</span>b<span class="token punctuation">]</span>
      <span class="token punctuation">(</span>cons a b<span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
</code></pre>
<h1 id="ausgewählte-kapitel">4. Ausgewählte Kapitel</h1>
<h2 id="datenabstraktion">Datenabstraktion</h2>
<ul>
<li><strong>Es gibt keinen Unterschied zwischen Programmen und Daten</strong></li>
<li>Datentypen kann man bauen und damit unabhängig von festgelegten Repräsentationen rechnen</li>
</ul>
<h2 id="metazirkulärer-interpreter">Metazirkulärer Interpreter</h2>
<ul>
<li>Interpreter, der in derselben Sprache geschrieben ist, die er interpretiert</li>
<li>Prozess der Funktionsanwendung durch <code>eval</code> und <code>apply</code></li>
<li><code>eval</code> wertet den Ausdruck aus und gibt das Ergebnis zurück</li>
<li><code>apply</code> erwartet eine Funktion und eine Sequenz von Argumenten und wendet die Funktion auf die Elemente der Sequenz an</li>
<li><strong>Self-evaluation expression:</strong> Ausdruck, der sich selbst wieder als Ergebnis hat</li>
</ul>
<h2 id="lazy-evaluation">Lazy evaluation</h2>
<ul>
<li>auch: <em>call by need</em> oder <em>promises</em></li>
<li>Use-Case: Das Ergebnis einer aufwendigen Berechnung wird als Parameter benötigt (keinmal oder n-mal). Durch Lazy Evaluation wird der Wert nicht n-mal durchgeführt, sondern einmal und dann zwischengespeichert.</li>
</ul>
<h2 id="funktionale-datenstrukturen">Funktionale Datenstrukturen</h2>
<ul>
<li>Änderungen imperativer Datenstrukturen basieren auf Mutation</li>
<li>Funktionale Datenstrukturen sind nicht änderbar (immutable)</li>
<li>Änderungen von Werten erzeugen ein neues Exemplar der Datenstruktur</li>
<li>Kopien sorgen für eine lange Laufzeit</li>
<li><strong>Lösung:</strong> Baumstrukturen, zur Vermeidung von Redundanzen</li>
<li>Bei Änderung eines Werts werden die Knoten des Pfads zum Element kopiert</li>
<li>Verschiedene Fälle sind <a href="https://hypirion.com/musings/understanding-persistent-vector-pt-1">hier</a> zu finden.</li>
<li>Zur Beschleunigung der Operationen können Mehrwegbäume anstatt von Binärbäumen eingesetzt werden</li>
</ul>
<h4 id="beispiel">Beispiel</h4>
<p><a href="https://johbra.github.io/PP2/Vorlesung/Abbildungen/vec2.png"><img src="https://johbra.github.io/PP2/Vorlesung/Abbildungen/vec2.png" alt="Beispiel eines kopierten Pfads"></a></p>
<h1 id="funktionale--vs.-objektorientierte-programmierung">5. Funktionale- vs. Objektorientierte Programmierung</h1>

<table>
<thead>
<tr>
<th align="center">Funktionale Programmierung</th>
<th align="center">Objektorientierte Programmierung</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">Fehlen von Mutation</td>
<td align="center">Gebrauch von Mutation</td>
</tr>
<tr>
<td align="center">Fehlen von Zuweisungen</td>
<td align="center">Gebrauch von Zuweisungen</td>
</tr>
<tr>
<td align="center">Funktionen</td>
<td align="center">Objekte (Funktionen mit internen Daten)</td>
</tr>
<tr>
<td align="center">Funktionen</td>
<td align="center">Methoden</td>
</tr>
</tbody>
</table><h3 id="zusammenfassung">Zusammenfassung:</h3>
<ul>
<li>Für eine “objektorientierte Programmierung” bedarf es keiner speziellen Programmiersprache</li>
<li>Objekte sind:
<ul>
<li>eine Menge von Key-Value-Abbildungen</li>
<li>eine Reihe von Funktionen, die Key-Value-Abbildungen akzeptieren</li>
<li>eine Verteilfunktion zum Aufruf der gewünschten Funktion</li>
</ul>
</li>
<li>Verwendung beider Paradigmen abhängig vom Anwendungskontext und persönlichem Geschmack</li>
<li>Aufwand der Erweiterbarkeit der Paradigmen sollte ebenfalls in Betracht gezogen werden</li>
</ul>
<h2 id="objektorientiert-vs.-prozedural-vs.-funktional">Objektorientiert vs. Prozedural vs. Funktional</h2>
<h3 id="objektorientiert">Objektorientiert</h3>
<p><a href="https://johbra.github.io/PP2/Vorlesung/Abbildungen/gops-oop-markiert.png"><img src="https://johbra.github.io/PP2/Vorlesung/Abbildungen/gops-oop-markiert.png" alt=""></a></p>
<h3 id="prozedural">Prozedural</h3>
<p><a href="https://johbra.github.io/PP2/Vorlesung/Abbildungen/gops-proz-markiert.png"><img src="https://johbra.github.io/PP2/Vorlesung/Abbildungen/gops-proz-markiert.png" alt=""></a></p>
<h3 id="funktional">Funktional</h3>
<p><a href="https://johbra.github.io/PP2/Vorlesung/Abbildungen/gops-schluss.png"><img src="https://johbra.github.io/PP2/Vorlesung/Abbildungen/gops-schluss.png" alt=""></a></p>
<h2 id="funktionale-entwurfsmuster">Funktionale Entwurfsmuster</h2>
<ul>
<li>
<h3 id="command-pattern">Command-Pattern</h3>
<ul>
<li>Modularisierung von Befehlen und Aufrufen</li>
</ul>
</li>
<li>
<h3 id="strategy-pattern">Strategy-Pattern</h3>
<ul>
<li>Flexibler Wechsel von alternativen Verhalten</li>
</ul>
</li>
<li>
<h3 id="oberserver-pattern">Oberserver-Pattern</h3>
<ul>
<li>Benachrichtigung einer oder mehrerer Objekte, wenn sich der Zustand eines bestimmten Objekts ändert</li>
</ul>
</li>
</ul>
<h1 id="funktionale-konzepte-in-java">6. Funktionale Konzepte in Java</h1>
<blockquote>
<p>Gilt nur für Java 8 oder größer!</p>
</blockquote>
<ul>
<li>z.B. <code>map</code>, <code>filter</code> und <code>reduce</code></li>
<li>Vermeidung expliziter Mutation</li>
<li>lesbarer Code</li>
<li>Formulierung <strong>was</strong> (deklerativ) geschehen soll, nicht <strong>wie</strong> (imperativ)</li>
<li>Objektorientierung steht nicht im Widerspruch zur Funktionalen Programmierung</li>
</ul>
<h3 id="funktionale-interfaces-in-java">Funktionale Interfaces in Java</h3>
<ul>
<li><code>Consumer&lt;T&gt;</code> - Operation ohne Rückgabe</li>
<li><code>Supplier&lt;T&gt;</code> - Fabrik, die ein neues oder existierendes Objekt liefert</li>
<li><code>Predicate&lt;T&gt;</code> - Prüfung einer Bedingung für ein Argument</li>
<li><code>Function&lt;T&gt;</code> - Operation mit Resultat</li>
</ul>
<h2 id="fluent-interfaces">Fluent Interfaces</h2>
<ul>
<li>Objektorientierte API unter Verwendung von method chaining</li>
</ul>
<h3 id="verwendung-von-fluent-interfaces-am-beispiel">Verwendung von Fluent Interfaces am Beispiel:</h3>
<pre class=" language-java"><code class="prism  language-java"><span class="token keyword">public</span> <span class="token keyword">static</span> <span class="token keyword">void</span> <span class="token function">main</span><span class="token punctuation">(</span><span class="token keyword">final</span> String<span class="token punctuation">[</span><span class="token punctuation">]</span> args<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	FluentMailer<span class="token punctuation">.</span><span class="token function">send</span><span class="token punctuation">(</span>mailer <span class="token operator">-</span><span class="token operator">&gt;</span>
		mailer<span class="token punctuation">.</span><span class="token function">from</span><span class="token punctuation">(</span><span class="token string">"build@agiledeveloper.com"</span><span class="token punctuation">)</span>
			<span class="token punctuation">.</span><span class="token function">to</span><span class="token punctuation">(</span><span class="token string">"venkats@agiledeveloper.com"</span><span class="token punctuation">)</span>
			<span class="token punctuation">.</span><span class="token function">subject</span><span class="token punctuation">(</span><span class="token string">"build notification"</span><span class="token punctuation">)</span>
            <span class="token punctuation">.</span><span class="token function">body</span><span class="token punctuation">(</span><span class="token string">"...much better..."</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
  <span class="token punctuation">}</span>
</code></pre>
<h1 id="relationale-programmierung">7. Relationale Programmierung</h1>
<h1 id="relational-logische-programmierung">8. Relational-logische Programmierung</h1>
<h1 id="constraint-programmierung---grundlagen">9. Constraint Programmierung - Grundlagen</h1>
<h1 id="constraint-solving">10. Constraint-solving</h1>
<h1 id="constraint-logic-programmierung">10. Constraint-logic Programmierung</h1>
<h1 id="parallelprogrammierung">11. Parallelprogrammierung</h1>
<h2 id="einstieg">Einstieg</h2>
<h2 id="multithreading-in-java">Multithreading (in Java)</h2>
<h2 id="software-transactional-memory">Software Transactional Memory</h2>
<h2 id="parallele-algorithmen">Parallele Algorithmen</h2>

