# Sensitive-Data-Scraping
This repo is dedicated to all the regexes which I searched and found on multiple blogs/repos/articles for scraping sensitive data out of a page/site.

Reference :- https://github.com/dxa4481/truffleHogRegexes

<h5>Regex table for sensitive information harvesting</h5>
<table class="wrapped">
    <colgroup>
        <col />
        <col />
    </colgroup>
    <tbody>
        <tr>
            <td>
                <p><strong>Slack Token</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(xox[p|b|o|a]-[0-9]{12}-[0-9]{12}-[0-9]{12}-[a-z0-9]{32})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>RSA private key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">-----BEGIN RSA PRIVATE KEY-----</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>SSH (OPENSSH) private key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">-----BEGIN OPENSSH PRIVATE KEY-----</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>SSH (DSA) private key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">-----BEGIN DSA PRIVATE KEY-----</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>SSH (EC) private key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">-----BEGIN EC PRIVATE KEY-----</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>PGP private key block</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">-----BEGIN PGP PRIVATE KEY BLOCK-----</span></p>
            </td>
        </tr>
        <tr>
            <td colspan="1"><strong>Putty Key</strong></td>
            <td colspan="1"><span style="color: rgb(0,0,255);">PuTTY-User-Key-File-2</span></td>
        </tr>
        <tr>
            <td colspan="1"><strong>SSH2 private key</strong></td>
            <td colspan="1"><span style="color: rgb(0,0,255);">-----BEGIN SSH2 ENCRYPTED PRIVATE KEY-----</span></td>
        </tr>
        <tr>
            <td>
                <p><strong>Generic Private Key block</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">BEGIN.*PRIVATE KEY</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Username Password combo</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">^[a-z]+://.*:.*@</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Facebook Oauth</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">[f|F][a|A][c|C][e|E][b|B][o|O][o|O][k|K].*['|\&quot;][0-9a-f]{32}['|\&quot;]</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Twitter Oauth</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">[t|T][w|W][i|I][t|T][t|T][e|E][r|R].*['|\&quot;][0-9a-zA-Z]{35,44}['|\&quot;]</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>GitHub</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">[g|G][i|I][t|T][h|H][u|U][b|B].*['|\&quot;][0-9a-zA-Z]{35,40}['|\&quot;]</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google Oauth</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(\&quot;client_secret\&quot;:\&quot;[a-zA-Z0-9-_]{24}\&quot;)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>AWS API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">AKIA[0-9A-Z]{16}</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Heroku API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">[h|H][e|E][r|R][o|O][k|K][u|U].*[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12}</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Generic API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">[a|A][p|P][i|I][_]?[k|K][e|E][y|Y].*['|\&quot;][0-9a-zA-Z]{32,45}['|\&quot;]</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Generic Secret</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">[s|S][e|E][c|C][r|R][e|E][t|T].*['|\&quot;][0-9a-zA-Z]{32,45}['|\&quot;]</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Slack Webhook</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">https://hooks[.]slack[.]com/services/T[a-zA-Z0-9_]{8}/B[a-zA-Z0-9_]{8}/[a-zA-Z0-9_]{24}</span>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google (GCP) Service-account</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">\&quot;type\&quot;: \&quot;service_account\&quot;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Twilio API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">SK[a-z0-9]{32}</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Password in URL</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">[a-zA-Z]{3,10}://[^/\\s:@]{3,20}:[^/\\s:@]{3,20}@.{1,100}[\&quot;'\\s]</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Amazon MWS Auth Token</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(amzn\\.mws\\.[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Facebook Access Token</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(EAACEdEose0cBA[0-9A-Za-z]+)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(AIza[0-9A-Za-z\\-_]{35})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google Cloud Platform API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(AIza[0-9A-Za-z\\-_]{35})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Password in URL</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">[a-zA-Z]{3,10}://[^/\\s:@]{3,20}:[^/\\s:@]{3,20}@.{1,100}[\&quot;'\\s]</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google Cloud Platform OAuth</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">([0-9]+-[0-9A-Za-z_]{32}\\.apps\\.googleusercontent\\.com)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google Drive API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(AIza[0-9A-Za-z\\-_]{35})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google Drive OAuth</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">([0-9]+-[0-9A-Za-z_]{32}\\.apps\\.googleusercontent\\.com)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google (GCP) Service-account</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">("type": "service_account".*)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google Gmail API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(AIza[0-9A-Za-z\\-_]{35})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google Gmail OAuth</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">([0-9]+-[0-9A-Za-z_]{32}\\.apps\\.googleusercontent\\.com)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google OAuth Access Token</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(ya29\\.[0-9A-Za-z\\-_]+)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google YouTube API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(AIza[0-9A-Za-z\\-_]{35})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Google YouTube OAuth</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">([0-9]+-[0-9A-Za-z_]{32}\\.apps\\.googleusercontent\\.com)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>MailChimp API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">([0-9a-f]{32}-us[0-9]{1,2})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Mailgun API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(key-[0-9a-zA-Z]{32})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>PayPal Braintree Access Token</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(access_token\\$production\\$[0-9a-z]{16}\\$[0-9a-f]{32})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Picatic API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(sk_live_[0-9a-z]{32})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Stripe API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(sk_live_[0-9a-zA-Z]{24})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Stripe Restricted API Key</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(rk_live_[0-9a-zA-Z]{24})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Square Access Token</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(sq0atp-[0-9A-Za-z\\-_]{22})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Square OAuth Secret</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">(sq0csp-[0-9A-Za-z\\-_]{43})</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Twitter Access Token</strong></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">([t|T][w|W][i|I][t|T][t|T][e|E][r|R].*[1-9][0-9]+-[0-9a-zA-Z]{40})</span></p>
            </td>
        </tr>
    </tbody>
</table>
<h5>Blacklisted Keywords to search for inside the context</h5>
<table class="wrapped">
    <colgroup>
        <col />
    </colgroup>
    <tbody>
        <tr>
            <th>
                <p><span style="color: rgb(0,0,255);"><strong>apikey</strong></span></p>
            </th>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);"><strong>api_key</strong></span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);"><strong>aws_secret_access_key</strong></span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);"><strong>db_pass</strong></span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);"><strong>password</strong></span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);"><strong>passwd</strong></span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);"><strong>private_key</strong></span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);"><strong>secret</strong></span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);"><strong>secrete</strong></span></p>
            </td>
        </tr>
    </tbody>
</table>
<h5><span style="color: rgb(94,108,132);">Considering the False Positives cases</span></h5>
<table class="wrapped">
    <colgroup>
        <col />
    </colgroup>
    <tbody>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">&quot;&quot;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">&quot;&quot;):</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">&quot;\'</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">&quot;)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">#pass</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">#password</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">$(shell</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">'\&quot;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">''</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">''):</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">')</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">'this</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">(nsstring</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">-default}</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">&lt;a</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">&lt;aws_secret_access_key&gt;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">&lt;input</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">&lt;password&gt;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">=</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">\\&quot;$(shell</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">\\k.*&quot;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">\\k.*'</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">`grep</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">dummy_secret</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">false</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">false):</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">false,</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">false;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">none</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">none,</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">none}</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">not</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">null</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">null,</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">null;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">password</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">password)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">password,</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">password},</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">redacted</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">some_key</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">string,</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">string?</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">string}</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">string}}</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">test-access-key</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">todo</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">true</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">true):</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">true,</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">true;</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><span style="color: rgb(0,0,255);">{</span></p>
            </td>
        </tr>
    </tbody>
</table>
<h5><span style="color: rgb(94,108,132);">Regex for Specific Cases</span></h5>
<table class="wrapped">
    <colgroup>
        <col />
        <col />
    </colgroup>
    <tbody>
        <tr>
            <td>
                <p><strong>Something followed by Colon</strong></p>
                <p><em>Eg. secret_key: foo</em></p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">({})((&quot;|\')?):(\s*?)((&quot;|\')?)([^\s]+)(\5)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Something followed by Colon &amp; Quotes</strong></p>
                <p><em><em>Eg. </em>secret_key: &quot;foo&quot;</em>
                </p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">({})((&quot;|\')?):(\s*?)((&quot;|\'))([^\s]+)(\5)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Something followed by Equal signs</strong></p>
                <p><em><em>Eg. </em>password = bar</em>
                </p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">({})((\'|&quot;)])?()(\s*?)=(\s*?)((&quot;|\')?)([^\s]+)(\7)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Something followed by Equal signs &amp; Quotes</strong></p>
                <p><em><em>Eg. </em>password = &quot;bar&quot;</em>
                </p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">({})((\'|&quot;)])?()(\s*?)=(\s*?)((&quot;|\'))([^\s]+)(\7)</span></p>
            </td>
        </tr>
        <tr>
            <td>
                <p><strong>Something followed by Quotes &amp; Semicolon</strong></p>
                <p><em><em>Eg. </em>private_key &quot;something&quot;;</em>
                </p>
            </td>
            <td>
                <p><span style="color: rgb(0,0,255);">({})([^\s]*?)(\s*?)(&quot;|\')([^\s]+)(\4);</span></p>
            </td>
        </tr>
    </tbody>
</table>
<p><br /></p>
<p><br /></p>
