<h2>Zugriff auf den Server</h2>
<p><strong>User / Password</strong></p>
<p>Der User ist <code>ubuntu</code>, dass Password steht in der Datei <a href="/data/.ssh/passwd">/data/.ssh/passwd</a>.</p>
<p>Einloggen mittels</p>
<pre><code>ssh ubuntu@${ADDR}</code></pre>
<p><strong>SSH</strong></p>
<p>Auf der Server kann mittels <a href="https://wiki.ubuntuusers.de/SSH/">ssh</a> zugegriffen werden.</p>
<p>Der private SSH Key ist auf dem installierten Server unter <a href="/data/.ssh/id_rsa">/data/.ssh/id_rsa</a> zu finden. Downloaden und dann wie folgt auf den Server einloggen:</p>
<pre><code>ssh -i id_rsa ubuntu@${ADDR}</code></pre>
<p><strong>Hinweis</strong>: Windows User verwenden <a href="https://www.bitvise.com/">bitvise</a> und legen den privaten SSH Key im "Client key manager" ab. Sollten Sie die Command-Line verwenden erhalten Sie unter Umständen einen Fehler "invalid Format". Windows erwartet am Ende des private Key eine Leerzeile. Fügen Sie diese dem Key hinzu, dann geht das Login auch via Command-Line.</p>
<p><strong>Shell in a Box (web based terminal emulator)</strong></p>
<p>Mittels Shell in a Box kann via Browser auf die VM zugegriffen werden. Die Installation eines Terminal Emulators (wie bitvise) entfällt.</p>
<p>Der URL ist <a href="https://${ADDR}:4200">https://${ADDR}:4200</a>.</p>
<p>User und Password siehe oben.</p>