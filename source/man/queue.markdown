---
layout: legacy
title: puppet queue Manual Page
---

puppet queue Manual Page
======

<div class='mp'>
<h2 id="NAME">NAME</h2>
<p class="man-name">
  <code>puppet-queue</code> - <span class="man-whatis">Queuing daemon for asynchronous storeconfigs</span>
</p>

<h2 id="SYNOPSIS">SYNOPSIS</h2>

<p>Retrieves serialized storeconfigs records from a queue and processes
them in order.</p>

<h2 id="USAGE">USAGE</h2>

<p>puppet queue [-d|--debug] [-v|--verbose]</p>

<h2 id="DESCRIPTION">DESCRIPTION</h2>

<p>This application runs as a daemon and processes storeconfigs data,
retrieving the data from a stomp server message queue and writing it to
a database.</p>

<p>For more information, including instructions for properly setting up
your puppet master and message queue, see the documentation on setting
up asynchronous storeconfigs at:
http://projects.puppetlabs.com/projects/1/wiki/Using_Stored_Configuration</p>

<h2 id="OPTIONS">OPTIONS</h2>

<p>Note that any configuration parameter that's valid in the configuration
file is also a valid long argument. For example, 'server' is a valid
configuration parameter, so you can specify '--server <var>servername</var>' as
an argument.</p>

<p>See the configuration file documentation at
http://docs.puppetlabs.com/references/stable/configuration.html for the
full list of acceptable parameters. A commented list of all
configuration options can also be generated by running puppet queue with
'--genconfig'.</p>

<dl>
<dt class="flush">--debug</dt><dd><p>Enable full debugging.</p></dd>
<dt class="flush">--help</dt><dd><p>Print this help message</p></dd>
<dt>--verbose</dt><dd><p>Turn on verbose reporting.</p></dd>
<dt>--version</dt><dd><p>Print the puppet version number and exit.</p></dd>
</dl>


<h2 id="EXAMPLE">EXAMPLE</h2>

<pre><code>$ puppet queue
</code></pre>

<h2 id="AUTHOR">AUTHOR</h2>

<p>Luke Kanies</p>

<h2 id="COPYRIGHT">COPYRIGHT</h2>

<p>Copyright (c) 2011 Puppet Labs, LLC Licensed under the Apache 2.0 License</p>

</div>
