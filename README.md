<h1 align="center">🚀 PretextRenderLab</h1>
<p align="center">
  Experimental UI Systems for <b>Zero-DOM-Reflow Rendering</b>
</p>

<hr/>

<h2>🧠 Overview</h2>
<p>
Modern web UIs often suffer from <b>layout thrashing</b> due to repeated DOM measurements 
(<code>getBoundingClientRect</code>, <code>offsetHeight</code>, etc.).
</p>

<p>
This project explores an alternative approach:
</p>

<p><b>Precompute layout using canvas → eliminate DOM reads → achieve zero reflows.</b></p>

<hr/>

<h2>⚡ Key Features</h2>
<ul>
  <li>🧮 <b>Canvas-based Text Measurement</b> using <code>canvas.measureText()</code></li>
  <li>🚫 <b>Zero DOM Reflows</b> (no layout-triggering reads)</li>
  <li>🧱 <b>Precomputed Layout Engine</b></li>
  <li>🧵 <b>Virtualized Rendering</b> (only visible elements rendered)</li>
  <li>📊 <b>Live Performance Metrics</b></li>
</ul>

<hr/>

<h2>🚀 Live Demo</h2>
<ul>
  <li><a [href="https://your-link.netlify.app](https://chronicalpretext.netlify.app)">Chronicle Feed</a></li>
  <li><a "https://chronicalpretext.netlify.app">Virtualized Chat</a></li>
</ul>

<h2>📂 Projects</h2>

<h3>📰 Chronicle — Pretext Masonry Feed</h3>
<ul>
  <li>Masonry layout with precomputed heights</li>
  <li>500 dynamic articles</li>
  <li>Zero reflows during layout</li>
  <li>Live performance HUD</li>
</ul>

<h3>💬 Virtualized Chat Engine</h3>
<ul>
  <li>10,000-item chat simulation</li>
  <li>Pretext vs DOM comparison</li>
  <li>FPS + benchmark visualization</li>
</ul>

<hr/>

<hr/>

<h2>📊 Performance Comparison</h2>

<table>
  <tr>
    <th>Metric</th>
    <th>DOM Approach</th>
    <th>Pretext Approach</th>
  </tr>
  <tr>
    <td>Layout Measurement</td>
    <td>DOM Reads</td>
    <td><b>Canvas</b></td>
  </tr>
  <tr>
    <td>Reflows</td>
    <td>High</td>
    <td><b>Zero</b></td>
  </tr>
  <tr>
    <td>Scalability</td>
    <td>Poor</td>
    <td><b>Excellent</b></td>
  </tr>
</table>

<hr/>

<h2> Core Idea</h2>

<p>Instead of:</p>

<pre><code>element.getBoundingClientRect()</code></pre>

<p>We use:</p>

<pre><code>canvas.measureText()</code></pre>

<p>
Then compute layout mathematically and render only visible elements.
</p>

<hr/>

<h2> Architecture</h2>

<pre><code>
Input Data
   ↓
Canvas Text Measurement
   ↓
Height Calculation
   ↓
Layout Engine
   ↓
Virtualized Rendering
   ↓
DOM (write-only)
</code></pre>

<hr/>

<h2>💡 Why This Matters</h2>
<ul>
  <li>Eliminates layout thrashing</li>
  <li>Improves performance at scale</li>
  <li>Gives developers full control over layout</li>
</ul>

<hr/>

<hr/>

<h2>Author</h2>
<p>
<b>Divya Rajput</b><br/>
</p>

<hr/>

<p align="center">
  ⭐ If you find this interesting, consider starring the repo!
</p>
