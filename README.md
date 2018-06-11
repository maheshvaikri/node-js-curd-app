<p><strong>Disclaimer:</strong> Understanding of JavaScript, MongoDB, HTML and CSS | Full-Stack Web Development is a pre-requisite.</p>

<br/>

<h1>CRUD (Create, Read, Update and Delete) Application in NodeJS</h1>
<p>Node.js is a JavaScript library to write server-side scripts. <br/> Before it, JavaScript was used for client side script to run on browser, but Node.js enabled us to write server-side scripts running on server to delivery dynamic web pages to client's browser.</p>

<br/>

<h3>TERMINOLOGIES &amp; INSTALLATION</h3>
<p>Follow through following installation instruction and terminologies to understand how the code attached with this git or to create your own application in Node.</p>
<ul>
	<li>
	<p>Download and Install Node.js from <a target="_blank" href="https://nodejs.org/en/download/">Download Node.js</a>.</p>
	<p>After installing Node.js navigate to your project directory and run following commands in terminal to initialize project:</p>
		<pre><strong><code>
			npm init
		</code></strong></pre>
	<p>Running above command will ask you few question - enter project name and press enter for all. You will find <strong>package.json</strong> file, open it in editor and replace following line to set Node start command and specify start page:</p>
		<pre><strong><code>
			"test": "echo \"error..."
		</code></strong></pre>
		to
		<pre><strong><code>
			"start": "node index"
		</code></strong></pre>
	<p>Next, create a blank <strong>index.js</strong> file in the same directory. This is the start page.</p>
	<p>Now, you can run your Node.js application by running following commands in terminal:</p>
		<pre><strong><code>
			node start
		</code></strong></pre>
	<p>However, we are going to use <strong>nodemon</strong> to run Node.js application. Install by running following command:</p>
		<pre><strong><code>
			npm install -g nodemon
		</code></strong></pre>
	<p>Now you can start your application with command: <code><strong>nodemon</strong></code>. The beauty is that the code will be auto-compiled and executed after saving, saving you the hassle of restarting the server every time you modify your code as in case of <strong><code>start node</code></strong>.</p>
	</li>

	<br/>

	<li>
	<p><strong>Express</strong> is a Node.js framework that simplifies the work of Node.js. Read about it from: <a target="_blank" href="https://expressjs.com/">Express.js</a>.</p>
	<p>Run following commands to install express framework:</p>
		<pre><strong><code>
			npm install --save express
		</code></strong></pre>
	</li>

	<br/>

	<li>
	<p><strong>Pug</strong> is a template engine used instead of HTML. Read about it from: <a target="_blank" href="https://pugjs.org/api/getting-started.html">Pug.js</a></p>
	<p>Run following commands to install pug template engine:</p>
		<pre><strong><code>
			npm install --save pug
		</code></strong></pre>
	<p>Note: You can choose to convert HTML to Pug from <strong>HTML2Jade</strong> (<a href="html2jade.org/" target="_blank">html2jade.org</a>). Pug was originally known as Jade.</p>
	</li>

	<br/>

	<li>
	<p><strong>Mongoose</strong> is a npm package for MongoDB object modeling designed to work asynchronously. Read about it from: <a target="_blank" href="https://www.npmjs.com/package/mongoose">Mongoose</a></p>
	<p>Run following commands to install mongoose package:</p>
		<pre><strong><code>
			npm install --save mongoose
		</code></strong></pre>
		
	<p>Obviously, you need to have MongoDB installed and set up a database <strong>'nodejs_crud_app'</strong>. You can download and install from: <a target="_blank" href="https://www.mongodb.com/">MongoDB</a>.</p>
	</li>

	<br/>

	<li>
	<p><strong>Body Parser</strong> is npm package used to parse input form body in desired format. However, we will parse in JSON.</p>
	<p>Run following commands to install body parser package:</p>
		<pre><strong><code>
			npm install --save body-parser
		</code></strong></pre>
	</li>
	
	<br/>
	
	<li>
	<p><strong>Bower</strong> is a package manager like npm for installing packages like bootstrap, jquery, etc.</p>
	<p>Run following commands to install Bower package manager:</p>
		<pre><strong><code>
			npm install -g bower
		</code></strong></pre>
	<p>Note: We need to setup a installation for bower. To do so create a file called <strong>.bower.rc</strong> (note the '.') and put following line into it:</p>
		<pre><strong><code>
			{"directory":"public/bower_component"}
		</code></strong></pre>
	<p>We will not use it. But, it's good that you know it for building real-life applications.</p>
	</li>
	
	<br/>
	
	<li>
	<p>We will also need <strong>express-messages</strong> and <strong>connect-flash</strong> for flash message, <strong>express-session</strong> for user session and <strong>express-validator</strong> for validation. Install all using following command:</p>
		<pre><strong><code>
			npm install --save express-message express-session connect-flash express-validation
		</code></strong></pre>
	<p>Follow through all of their documentation online.</p>
	</li>
	
	<br/>
	
	<li>
	<p>Lastly, we will use <strong>passport</strong> for authentication. Read about it from : <a target="_blank" href="http://passportjs.org">passportjs.org</a>.</p>
	<p>Run following command to install passport authentication manager:</p>
		<pre><strong><code>
			npm install --save passport passport-local bcryptjs
		</code></strong></pre>
	<p>Above, <strong>passport-local</strong> is used to interact with local storage like MongoDB and <strong>bcrypt</strong> for encrypting passport.</p>
</ul>

<br/><br/>

<h3>LET'S WRITE THE CURD APP IN NODE JS</h3>
<p>I prefer the hard way, therefore, I am not going to explain you everything over here, but I will make sure that the code have enough documentation to explain you everything.</p>

<br/>

<h4>Download and Run Code:</h4>
<p>Download the code from this git repository and follow through all the code comments.</p>
<p>To run the downloaded code navigate to project directory in terminal and run command: <strong><code>nodemon</code></strong> and visit <a>http://localhost:3000/</a> in browser to see app running.</p>

<br/>

<h4>How does the code work?</h4>
<p>It's simple, just follow through all the code in a flow starting from </strong>"index.js"</strong> file and you can follow all codes easily. <br/> The code is commented to be easily understood.<p>

<br/>

<p>On a final note, let me know if you desire modification / found bug / have doubts at <a href="mailto:chettri@live.com">chettri@live.com</a>.</p>
