<h1>Basecoat Framework</h1>
Basecoat is an effort to create a small (~2,000 lines of code), fast, static free micro framework that can be loaded as an instance and used like a library. It makes no assumptions about how your code is structured or how it works. This makes migrating from an old code base to Basecoat very feasible. Your old code can run along side Basecoat while migrating. Acceleration and caching is not a necessity for good performance (600+ pages/sec with a plain install).

Basecoat continues to mature and is currently used by high traffic sites like footage.shutterstock.com, bigstockphoto.com and the Someecards' Facebook application. 

<h2>Why Another PHP Framework?</h2>
The most popular frameworks are tending towards large code bases that require caching and a code accelerators, like APC, in order to perform well. There is also a tendency towards using static classes and variables. Most frameworks force you to adopt their conventions and write your code "under" their framework.

Basecoat allows you to use raw PHP to develop you application. Namespacing and scoping are available to keep code modularized.

<h2>Features</h2>
<ul>
<li>Flexible, scalable router allowing hierarchies and anything to be loaded as a module</li>
<li>Automatic redirects between http/https by use of a route parameter</li>
<li>Template rendering as a module, allowing multiple renderings in a single request</li>
<li>PHP as a templating language. No need to learn a different syntax to take advantage of the templating</li>
<li>Flash message support</li>
<li>Database abstraction layer based on PDO. Support for multiple master/slave connections, built-in profiling and auto-escaping of data.</li>
<li>Hooks available to inject your own code at various stages</li>
<li>Simple configuration and no dependencies</li>
</ul>

<h2>Overview</h2>
Basecoat is designed to cover the basics: MVC, Front Controller, Templating, and Database abstraction. It is designed to be "included" in your code and using it as a full framework is optional. This allows one to build parts of a website in the framework and migrate over time. It does not enforce a coding style, naming convention, or have many dependencies. Basecoat is designed to be a centralized core code base that websites are built on. The same core code base can be loaded by many different web sites and/or applications. The configurations that dictate the framework's behavior are part of the your web site code, not the framework. Pulling in updates won't overwrite any of your own code. 

The entire framework is about 5 files and 2,000 lines of code. It comes with a quick start site template to get you started almost immediately. Performance is quite good, handling many hundreds of pages per second with no accelerators or caching. It requires no special setup or configuration, not even mod_rewrite. It can be configured to use parameter based URLs or if you want "pretty urls" using mod_rewrite or something similar.

<h2>Documentation</h2>
To get started, simply download the framework, including the examples. Place the whole framework in a web accessible directory and point your browser at basecoat/examples/docs/public/. The documentation is written using the framework, so you can view the code and see how it is working while you read through the documentation. The documentation is the same as that contained in the Wiki pages.

Once you are comfortable with the setup, you can move the framework directory to a centralized location that is not web accessible. The start building your web site(s)!

<h2>Quickstart</h2>
There is a quickstart directory in the examples directory that can be used as a template for creating new websites. Simply make a copy of the quickstart directory and modify it to fit the needs to your new website.
<ol>
<li>Make a copy of the quickstart directory and put it wherever you want your website</li>
<li>Edit the public/index.php to load basecoat.php from the proper location</li>
</ol>
Load your new site by pointing your browser at the public directory of your new site.

<h2>License</h2>
Copyright (C) 2011-2013 by Shutterstock Images, LLC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
