
# MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets



<p>We all know the phrase:&nbsp;&nbsp;<em>«Everything that gets on the Internet, remains in it forever and becomes publicly available.»</em></p>



<h4>Down to hidden content.</h4>



<p>The&nbsp;&nbsp;<code>2021 году</code>&nbsp;pandemic brought back popularity&nbsp;&nbsp;<code>QR-кодов</code>.&nbsp;For&nbsp; the first time&nbsp;<code>QR-коды</code>&nbsp;they were used in production in&nbsp;&nbsp;<code>1994 году</code>&nbsp;a subsidiary&nbsp;&nbsp;<code>Toyota</code>&nbsp;in Japan and introduced them at an assembly plant to control produced cars and parts for them.&nbsp;Unlike a barcode,&nbsp;&nbsp;<code>QR-код</code>&nbsp;it contains more information, which prompted the manufacturer to introduce innovations.&nbsp;The technology began to spread mainly in Asian countries, and in the&nbsp;&nbsp;<code>2003 году</code>&nbsp;Chinese company&nbsp;&nbsp;<a href="https://www.inspiry.com.cn/" target="_blank" rel="noreferrer noopener">Inspiry</a>&nbsp;&nbsp;developed a special reading mechanism&nbsp;&nbsp;<code>QR-кодов</code>that allowed it to be done quickly, which fueled its popularity.&nbsp;However, widespread use was already in the period of mass use of&nbsp;&nbsp;<em>tablets</em>&nbsp;&nbsp;and&nbsp;&nbsp;<em>smartphones.</em>when reading became available through the camera of the wearable device.</p>


<div class="wp-block-image">
<figure class="aligncenter"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/25ba8966d12ed4143f2b091391d4b3d8.png" alt="Devices from the Chinese company Inspiry" title="Devices from the Chinese company Inspiry"><figcaption>Devices from the Chinese company Inspiry</figcaption></figure></div>


<p>On the one hand, QR codes provide all the conveniences in payments&nbsp;&nbsp;<code>BTC</code>, since you can not spend half an hour on making a transfer.&nbsp;It is enough to point the smartphone at&nbsp;&nbsp;<code>QR-код</code>&nbsp;and the payment form with all the filled fields will be generated by itself, all that remains is to press the button with payment confirmation.</p>



<blockquote class="wp-block-quote"><p><code>Переводы</code>.&nbsp;&nbsp;<code>оплаты</code>.&nbsp;&nbsp;<code>QR-коды</code>&nbsp;just an irreplaceable thing and the most important thing is that all this&nbsp;&nbsp;<em><u>saves our time</u></em>&nbsp;.</p></blockquote>



<h4>There is one more important thing to remember:</h4>



<p><code>Googlebot</code>,&nbsp;&nbsp;<code>Bingbot</code>,&nbsp;&nbsp;<code>Baidubot</code>&nbsp;work&nbsp;&nbsp;<code>24/7</code>&nbsp;and at any time can store private data in their giant servers.</p>



<p>In search of hidden content from the depths of search engines, heroes in black hoodies, completely opposite to search bots, from the famous TV series Mr. Robot are connected&nbsp;&nbsp;<code>(Mr. Robot)</code>&nbsp;.</p>


<div class="wp-block-image">
<figure class="aligncenter"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/69782fe7678c1a1530864a5528c3d670.gif" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<blockquote class="wp-block-quote"><p><code>«MrRobotQR»</code>&nbsp;is&nbsp;&nbsp;<em>an open source script that automates the process from entering a search keyword to deriving the private key of a Bitcoin wallet.</em></p></blockquote>



<h4>Requires Python 3 and Bash to run the script</h4>



<p><em>Bash</em>&nbsp;script:&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/10MrRobotQR/mrrobotqr.sh" target="_blank" rel="noreferrer noopener">mrrobotqr.sh</a>&nbsp;&nbsp;automates the following steps:</p>



<p>Run&nbsp; the&nbsp;<em>Python</em>&nbsp;script:&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/10MrRobotQR/qrcrawler.py" target="_blank" rel="noreferrer noopener">qrcrawler.p&nbsp;</a><a href="http://qrcrawler.py/">y</a>&nbsp;&nbsp;with the specified&nbsp;&nbsp;<em><u>keywords</u></em>&nbsp;&nbsp;to search and scan&nbsp;&nbsp;<em><u>images</u></em>&nbsp;&nbsp;in&nbsp;&nbsp;<code>Google</code>,&nbsp;&nbsp;<code>Bing</code>&nbsp;and&nbsp;&nbsp;<code>Baidu</code>.</p>


<div class="wp-block-image">
<figure class="aligncenter"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/5675c4c22e1ec6ec6bea65601bdfc2c4.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<p>All found images will be uploaded to a folder&nbsp;&nbsp;<code>qrbooty</code>&nbsp;with subfolders for each search engine.&nbsp;The script then renames and moves the files from the subfolders to a folder&nbsp;&nbsp;<code>qrbooty</code>&nbsp;with unique names.</p>



<p>The next step is to run a&nbsp;&nbsp;<em>Python</em>&nbsp;script:&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/10MrRobotQR/qr2key.py" target="_blank" rel="noreferrer noopener">qr2key.py</a>&nbsp;&nbsp;to scan the downloaded&nbsp;&nbsp;<em>images</em>&nbsp;&nbsp;in the folder&nbsp;&nbsp;<code>qrbooty</code>&nbsp;for the presence&nbsp;&nbsp;<code>QR-кодов</code>&nbsp;and check if they contain the&nbsp;&nbsp;<em><u>private keys</u></em>&nbsp;of the &nbsp;Bitcoin wallet.&nbsp;All private keys will be saved to a text file:&nbsp;&nbsp;<code>keylist.txt</code>.</p>



<p>After re-processing, the script&nbsp;&nbsp;<em>removes duplicates</em>&nbsp;&nbsp;in&nbsp;&nbsp;<code>keylist.txt</code>&nbsp;and outputs&nbsp;&nbsp;<em>the unique key&nbsp;</em>&nbsp;to a new file:&nbsp;&nbsp;<code>keylist_unique.txt</code>&nbsp;, which will already contain all the&nbsp;&nbsp;<em><u>unique private keys&nbsp;</u></em>&nbsp;of the Bitcoin wallet.</p>



<h2>Installation and launch:</h2>



<p>Open&nbsp;&nbsp;<a href="https://github.com/demining/TerminalGoogleColab" target="_blank" rel="noreferrer noopener"><strong>[TerminalGoogleColab]</strong></a>&nbsp;.</p>



<p><a href="https://github.com/demining/CryptoDeepTools/tree/main/10MrRobotQR" target="_blank" rel="noreferrer noopener"><strong>Let’s use the «10MrRobotQR</strong>&nbsp;«</a>&nbsp;repository&nbsp;&nbsp;.</p>



<pre class="wp-block-code"><code>git clone https://github.com/demining/CryptoDeepTools.git

cd CryptoDeepTools/10MrRobotQR/

ls</code></pre>



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/f51fd621c0ffc06514564725b32c079d.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<h3>Install the ZBar barcode reader software package</h3>



<pre class="wp-block-code"><code>sudo apt install python3-dev python3-setuptools python3-pip libzbar0 libzbar-dev</code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/6e813a239da8012ba3b8db8250a3eb1c.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<h3>Install all the packages, modules and libraries we need:</h3>



<pre class="wp-block-code"><code>cat requirements.txt</code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/631ec882b66ba43a479d98f15d9e9136.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code>pip3 install -r requirements.txt</code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/34942294c35781f7f1757793789a2947.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<h2>File permissions:</h2>



<pre class="wp-block-code"><code>chmod +x mrrobotqr.sh
chmod +x qr2key.py
chmod +x qrcrawler.py</code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/9d2025b5e291d96c09c98f80dbf14d74.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<blockquote class="wp-block-quote"><p><code>"bitcoin qr"</code>&nbsp;—&nbsp;&nbsp;<em>keyword for search engines</em></p></blockquote>



<h2>Running a bash script:</h2>



<pre class="wp-block-code"><code>./<strong>mrrobotqr</strong>.sh "<strong>bitcoin</strong> <strong>qr</strong>"</code></pre>



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/eb13b4511fc91c8369fd38bb00252a05.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/f2158e874e3e9a2a83257ea7ad0606da.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/548c1a9fad698f309bc244c9ae9aebf4.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<p>We open and look at all saved unique keys in the file:&nbsp;<code>keylist_unique.txt</code></p>



<pre class="wp-block-code"><code>cat keylist_unique.txt</code></pre>



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/1640c4404be33a09a352823c63c4c3e4.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/da21b71aa2bdd72be785f9609f273d70.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/4b61b4219b42e13f24291e303fcbbaf1.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<figure class="wp-block-image"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/b55b61c29c47504769aaaef582e38401.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2>History of searches with a positive balance of BTC coins:</h2>



<p><a href="https://cryptodeep.ru/bitaddress.html" target="_blank" rel="noreferrer noopener">Let’s open bitaddress</a>&nbsp;and&nbsp;&nbsp;&nbsp;check:</p>


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/4bfe9b07bce9f2bf46b59c45f8b8b6ec.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>L4vNZ86Pp6mkEPSPz9EcELK8cp1BxP3LWjxh7QvDanuMQBUJT9cG</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>JhCAfiAbwJSa65c2EDCfC9fbEwyzZZb25</strong>
<strong>Total</strong> <strong>balance</strong>:   0.01393000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/8be842939714a4f9b3b53da80a2faf64.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets" title=""></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>L2HcNb8wPCQ2gpL4oT5Mn6cvKqfAFjCqK3qWquak9BvYasbgWxxF</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 18<strong>cif9QYoSPSrmv9MN157mUejyNMr5wYVx</strong>
<strong>Total</strong> <strong>balance</strong>:   0.01313000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/5141551704f3fe8781a73b8e16305de2.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>KwFs9DSx3qQbagnRiZ2niczs5QteL1bE13mBdXFGAW1He7BxQ9qz</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>KyUqCo3pbBHvCp7ZcBvUSEaTLBocUAoU3</strong>
<strong>Total</strong> <strong>balance</strong>:   0.03611000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/2faff9856edcf2d942b7a6eed71f13e4.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>L5CGhW2yDnq3pGQdKm3ocM3AE32EekoKkKN6DvUqstziayr1R79V</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>AuRL68EyKTFAafj98GR2oAi7b9abNr3ja</strong>
<strong>Total</strong> <strong>balance</strong>:   0.03602000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/98a6dcb52260e12b50851b6e6fcf00b3.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>L3sxBKQ8HbFAv2vshfsL6RTEX8zP9CLDzw9BCh6hd5VTiihoAX5n</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>H957muSj2Sn23Mnym5DEoYquQqviqc7Ch</strong>
<strong>Total</strong> <strong>balance</strong>:   0.03628000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/2acc0f8992b5393a0de2191fb384a645.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>KzpPtHkQbZj32Pxtoo31bPZtbVbVV5DASdmaFWawgrYXBxhfNoLj</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>PCLwUTMj6z7up1mDGbEbMVhaQif9xBB5M</strong>
<strong>Total</strong> <strong>balance</strong>:   0.03632000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/73f1c3d47655bf57c4bf975270c80b12.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>L1DoUbneUoNAMqFHeGyerzXyxwbzYWB1mD2JL8sn855EgZKJxC5d</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>N5rmtTVvtTkVPB8xJNPx3bbaS7kZX2kX</strong>
<strong>Total</strong> <strong>balance</strong>:   0.01466000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/8931ed4506bffc4e6709c5bad85b1ae6.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>KzcTCCpwMFu3yS5EBczmD9bv4GSD42vCoicJzCrZdm4eyYRvBiGE</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>WeWVwSsUDgtMagerivywQzmBbeL2ETVJ</strong>
<strong>Total</strong> <strong>balance</strong>:   0.03677000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/015d8d9ed35ebbd3be02683811b34c2a.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>Kydoae8uQDUjxVWqqgqzoTQtMYkA6x1MGiPTx76AuTzyxdBTAYHc</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>Mz7STzHf3JBuG4fvXuiz1brGRXF2C4R9R</strong>
<strong>Total</strong> <strong>balance</strong>:   0.03498000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="alignleft"><img src="./MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets - «CRYPTO DEEP TECH»_files/b658245dc40ee8133358c3d597534e9c.png" alt="MrRobotQR scan QR codes from search engines in search of private keys of Bitcoin Wallets"></figure></div>


<pre class="wp-block-code"><code><strong>Private</strong> <strong>Key</strong> <strong>WIF</strong>: <strong>KzWA3G6wyAdWSpACmJXAec76xhFxMPhnzwKLK3pk1gxm4RencWmo</strong>
<strong>Bitcoin</strong> <strong>Address</strong>: 1<strong>HnBT3t4AKBP54UDTNGJB39DAv7caf7HP1</strong>
<strong>Total</strong> <strong>balance</strong>:   0.01601000 <strong>BTC</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>This video was created for the&nbsp;&nbsp;<a href="https://cryptodeep.ru/" target="_blank" rel="noreferrer noopener"><strong>CRYPTO DEEP TECH</strong></a>&nbsp;portal &nbsp;to ensure the financial security of data and cryptography on elliptic curves&nbsp;&nbsp;<code>secp256k1</code>&nbsp;against weak signatures&nbsp;&nbsp;<code>ECDSA</code>&nbsp;in cryptocurrency&nbsp;<code>BITCOIN</code></p>



<p><strong><a href="https://github.com/demining/CryptoDeepTools/tree/main/10MrRobotQR" target="_blank" rel="noreferrer noopener">Source</a></strong></p>



<p><a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener"><strong>Telegram</strong></a><strong>&nbsp;:&nbsp;&nbsp;</strong><a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener"><strong><u>https://t.me/cryptodeeptech</u></strong></a></p>



<p><strong><a href="https://youtu.be/bNMg2iJhMpg" target="_blank" rel="noreferrer noopener">Video: https://youtu.be/bNMg2iJhMpg</a></strong></p>



<p><strong><a href="https://cryptodeeptech.ru/mr-robot-qr" target="_blank" rel="noreferrer noopener">Source: https://cryptodeeptech.ru/mr-robot-qr</a></strong></p>



---


|  | Donation Address |
| --- | --- |
| ♥ __BTC__ | 1Lw2gTnMpxRUNBU85Hg4ruTwnpUPKdf3nV |
| ♥ __ETH__ | 0xaBd66CF90898517573f19184b3297d651f7b90bf |

