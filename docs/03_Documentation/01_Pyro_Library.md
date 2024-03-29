
<div class="row-fluid">


<div class="span8">

<div id="main">



<h1 class="page-title">Class: Pyro</h1>
<section>

<header>
<h2>
Pyro
</h2>

</header>

<article>
<div class="container-overview">




<dt>
<h4 class="name" id="Pyro"><span class="type-signature"></span>new Pyro<span class="signature">(PyroData)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Enhanced functionality for the Firebase library</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>PyroData</code></td>


<td class="type">


<span class="param-type">object</span>



</td>





<td class="description last"><p>Object containing identifying information for creating a Pyro instance.</p>
<h6>Properties</h6>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>url</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Firebase url <code>Required</code></p></td>
</tr>



<tr>

<td class="name"><code>dbName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Database Name <code>Required</code></p></td>
</tr>



<tr>

<td class="name"><code>appUrl</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Hosted location of generated Pyro App <code>Not Required</code></p></td>
</tr>


</tbody>
</table>

</td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-1">line 1</a>
</li>
</ul>
</dd>







</dl>













</dd>


</div>














<h3 class="subsection-title">Methods</h3>

<dl>

<dt>
<h4 class="name" id="authAnonymously"><span class="type-signature"></span>authAnonymously<span class="signature">(onComplete)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Authenticate a user anonymously. Sessions are handled automatically.</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type"><a href="Pyro.html#authAnonymouslyCb">Pyro~authAnonymouslyCb</a></span>



</td>





<td class="description last"><p>Function called when completed</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-65">line 65</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="createInstance"><span class="type-signature"></span>createInstance<span class="signature">(listName, objectId, onComplete)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Create new instance of pyro</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>listName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>The name of the list the object will be put into.</p></td>
</tr>



<tr>

<td class="name"><code>objectId</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Key of object to be loaded</p></td>
</tr>



<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs on completion of delete operation</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-306">line 306</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="createObject"><span class="type-signature"></span>createObject<span class="signature">(listName, object, onComplete)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Creates an object provided the name of the list the object will go into and the object itself.
The object is created with a createdAt parameter that is a server timestamp from Firebase.
If a user is currently signed in, the object will contain the author's <code>$uid</code> under the author parameter. This is used for the getListByAuthor function.</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>listName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>The name of the list the object will be put into.</p></td>
</tr>



<tr>

<td class="name"><code>object</code></td>


<td class="type">


<span class="param-type">object</span>



</td>





<td class="description last"><p>Object you wish to create</p></td>
</tr>



<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type"><a href="Pyro.html#createObjectCb">Pyro~createObjectCb</a></span>



</td>





<td class="description last"><p>Function that runs when your object has been created successfully</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-169">line 169</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="deleteInstance"><span class="type-signature"></span>deleteInstance<span class="signature">(ListName, ObjectId, OnComplete)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Deletes pyro instance from list of instances</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>ListName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>The name of the list the object will be put into.</p></td>
</tr>



<tr>

<td class="name"><code>ObjectId</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Key of object to be loaded</p></td>
</tr>



<tr>

<td class="name"><code>OnComplete</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs on completion of delete operation</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-356">line 356</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="deleteObject"><span class="type-signature"></span>deleteObject<span class="signature">(listName, objectId, onSuccess, onError)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Deletes object given list name and object id</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>listName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>The name of the list the object will be put into.</p></td>
</tr>



<tr>

<td class="name"><code>objectId</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Key of object to be loaded</p></td>
</tr>



<tr>

<td class="name"><code>onSuccess</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs on completion of delete operation</p></td>
</tr>



<tr>

<td class="name"><code>onError</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs if delete operation fails <code>Returns</code> Error object</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-233">line 233</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="getAuth"><span class="type-signature"></span>getAuth<span class="signature">()</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Gets current auth information for main app reference</p>
</div>









<dl class="details">
<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-135">line 135</a>
</li>
</ul>
</dd>
</dl>













</dd>



<dt>
<h4 class="name" id="getListByAuthor"><span class="type-signature"></span>getListByAuthor<span class="signature">(listName, onComplete)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Gets list of objects created by the currently logged in User.</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>listName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>The name of the list the objects will be grabbed from.</p></td>
</tr>



<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs when the list has been retrieved successfully</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-150">line 150</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="getObjectCount"><span class="type-signature"></span>getObjectCount<span class="signature">(listName, onComplete, onError)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Get count of objects in a given list</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>listName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>The name of the list the object will be put into.</p></td>
</tr>



<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs on completion of gathering list count</p></td>
</tr>



<tr>

<td class="name"><code>onError</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs if there is an error</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-257">line 257</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="getUser"><span class="type-signature"></span>getUser<span class="signature">(onComplete)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Retreives account for currently logged in user</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type"><a href="global.html#getUserCb">getUserCb</a></span>



</td>





<td class="description last"><p>The name of the list the object will be put into.</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-189">line 189</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="getUserCount"><span class="type-signature"></span>getUserCount<span class="signature">(onComplete, onError)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Get user count</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs on completion of delete operation</p></td>
</tr>



<tr>

<td class="name"><code>onError</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs if there is an error</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-274">line 274</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="getUserList"><span class="type-signature"></span>getUserList<span class="signature">(onComplete, onError)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Get list of the users of your app</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs on completion of delete operation</p></td>
</tr>



<tr>

<td class="name"><code>onError</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs if there is an error</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-290">line 290</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="instanceRef"><span class="type-signature"></span>instanceRef<span class="signature">(listName, objectId, onComplete)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Reference to specific pyro instance</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>listName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>The name of the list the object will be put into.</p></td>
</tr>



<tr>

<td class="name"><code>objectId</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Key of object to be loaded</p></td>
</tr>



<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs on completion of delete operation</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-344">line 344</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="loadObject"><span class="type-signature"></span>loadObject<span class="signature">(listName, objectId, onSuccess, onError)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Loads object given list name and object id Notes: TO SIMILAR TO FIREBASE API</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>listName</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>The name of the list the object will be put into.</p></td>
</tr>



<tr>

<td class="name"><code>objectId</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Key of object to be loaded</p></td>
</tr>



<tr>

<td class="name"><code>onSuccess</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs on completion of load operation</p>
<h6>Properties</h6>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>ReturnValue</code></td>


<td class="type">


<span class="param-type">object</span>



</td>





<td class="description last"><p>Loaded object</p></td>
</tr>


</tbody>
</table>

</td>
</tr>



<tr>

<td class="name"><code>onError</code></td>


<td class="type">


<span class="param-type">function</span>



</td>





<td class="description last"><p>Function that runs if there is an error</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-214">line 214</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="login"><span class="type-signature"></span>login<span class="signature">(loginData)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Login a user with email and password</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>loginData</code></td>


<td class="type">

</td>





<td class="description last"><p>Login information for user</p>
<h6>Properties</h6>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>email</code></td>


<td class="type">

</td>





<td class="description last"><p>Email of user to login</p></td>
</tr>



<tr>

<td class="name"><code>password</code></td>


<td class="type">

</td>





<td class="description last"><p>Password of user to login</p></td>
</tr>


</tbody>
</table>

</td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-115">line 115</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="logout"><span class="type-signature"></span>logout<span class="signature">(onComplete)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Logout the current user from app Firebase</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>onComplete</code></td>


<td class="type">

</td>





<td class="description last"><p>Function that runs on completion of logout (Not Required)</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-125">line 125</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="userSignup"><span class="type-signature"></span>userSignup<span class="signature">(signupData)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Signup a new user with email and password. Sessions are handled automatically.</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>signupData</code></td>


<td class="type">


<span class="param-type">object</span>



</td>





<td class="description last"><p>Information of new user to signup</p>
<h6>Properties</h6>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>email</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Email of new user</p></td>
</tr>



<tr>

<td class="name"><code>password</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Password of new user</p></td>
</tr>


</tbody>
</table>

</td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-104">line 104</a>
</li>
</ul>
</dd>







</dl>













</dd>

</dl>



<h3 class="subsection-title">Type Definitions</h3>

<dl>

<dt>
<h4 class="name" id="authAnonymouslyCb"><span class="type-signature"></span>authAnonymouslyCb<span class="signature">(auth)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Callback used by authAnonymously</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>auth</code></td>


<td class="type">


<span class="param-type">object</span>



</td>





<td class="description last"><p>Anonymous auth information</p>
<h6>Properties</h6>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>uid</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Unique id of anonymous user</p></td>
</tr>



<tr>

<td class="name"><code>provider</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Login provider of user</p></td>
</tr>


</tbody>
</table>

</td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-90">line 90</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="createObjectCb"><span class="type-signature"></span>createObjectCb<span class="signature">(newObjRef)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>Callback function used by createObject</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>newObjRef</code></td>


<td class="type">


<span class="param-type">object</span>



</td>





<td class="description last"><p>Firebase reference created by new object</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-179">line 179</a>
</li>
</ul>
</dd>







</dl>













</dd>



<dt>
<h4 class="name" id="errorCb"><span class="type-signature"></span>errorCb<span class="signature">(errorObj, error, message)</span><span class="type-signature"></span></h4>


</dt>
<dd>


<div class="description">
<p>General error callback</p>
</div>







<h5>Parameters:</h5>


<table class="params table table-striped">
<thead>
<tr>

<th>Name</th>


<th>Type</th>





<th class="last">Description</th>
</tr>
</thead>

<tbody>


<tr>

<td class="name"><code>errorObj</code></td>


<td class="type">


<span class="param-type">object</span>



</td>





<td class="description last"><p>Object containing error information</p></td>
</tr>



<tr>

<td class="name"><code>error</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Error string</p></td>
</tr>



<tr>

<td class="name"><code>message</code></td>


<td class="type">


<span class="param-type">string</span>



</td>





<td class="description last"><p>Error message to display to users</p></td>
</tr>


</tbody>
</table>




<dl class="details">





















<dt class="tag-source">Source:</dt>
<dd class="tag-source">
<ul class="dummy">
<li>
<a href="pyro.js.html">pyro.js</a>,
<a href="pyro.js.html#sunlight-1-line-53">line 53</a>
</li>
</ul>
</dd>







</dl>













</dd>

</dl>



</article>

</section>




</div>

<div class="clearfix"></div>




</div>
<!--<script src="scripts/sunlight.js"></script>-->
<script src="../js/docstrap/docstrap.lib.js"></script>
<!-- <script src="../js/docstrap/bootstrap-dropdown.js"></script> -->
<script src="../js/docstrap/toc.js"></script>

<script>
$( function () {
  $( "[id*='$']" ).each( function () {
    var $this = $( this );

    $this.attr( "id", $this.attr( "id" ).replace( "$", "__" ) );
    } );

    $( "#toc" ).toc( {
      anchorName  : function ( i, heading, prefix ) {
        return $( heading ).attr( "id" ) || ( prefix + i );
        },
        selectors   : "h1,h2,h3,h4",
        showAndHide : false,
        scrollTo    : "100px"
        } );

        $( "#toc>ul" ).addClass( "nav nav-pills nav-stacked" );
        $( "#main span[id^='toc']" ).addClass( "toc-shim" );
        $( '.dropdown-toggle' ).dropdown();
        //			$( ".tutorial-section pre, .readme-section pre" ).addClass( "sunlight-highlight-javascript" ).addClass( "linenums" );

        $( ".tutorial-section pre, .readme-section pre" ).each( function () {
          var $this = $( this );

          var example = $this.find( "code" );
          exampleText = example.html();
          var lang = /{@lang (.*?)}/.exec( exampleText );
          if ( lang && lang[1] ) {
            exampleText = exampleText.replace( lang[0], "" );
            example.html( exampleText );
            lang = lang[1];
            } else {
              lang = "javascript";
            }

            if ( lang ) {

              $this
              .addClass( "sunlight-highlight-" + lang )
              .addClass( "linenums" )
              .html( example.html() );

            }
            } );

            Sunlight.highlightAll( {
              lineNumbers : true,
              showMenu : true,
              enableDoclinks : true
              } );
              } );
              </script>



              <!--Navigation and Symbol Display-->



              <!--Google Analytics-->


              </body>
              </html>
