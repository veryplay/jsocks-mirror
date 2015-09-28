Implements RFC1928 SOCKS protocol in both server and client form.  Pure Java implementation that is easy to understand and easy to modify.

Some features:
  1. RFC1929 SOCKS 5 Auth
  1. SOCKS4 protocol
  1. Client code supports ATYP = 3 (DNS remote resolution).
  1. Full server implemenation.  Its easy to create SOCKS servers that have custom authentication and firewall mechanisms.  This is a great way to write custom VPN type software:

This is a mirror from the JSOCKS sourceforge project.  That project has had no updates since 2000.  If I can get a hold of Kirill, I will delete this project.

Google has made updates and is using this mirror to distribute our changes per the LGPL.  Overall though, I hope we can continue to move this project forward.

Some changes Google has made:
  * Java style package names
  * Fixes to SOCKS client to support JDK 1.4 sockets concept of "connect()"
  * Log 4J logging instead of system.out.
  * Better logging statements through the ProxyServer class.

Original JSOCKS Sourceforge Project Page: https://sourceforge.net/projects/jsocks/

Original JSOCKS homepage: http://jsocks.sourceforge.net


Original JSOCKS homepage text:


---


<h1>
JAVA SOCKS Server</h1>
It is a SOCKS server written entirely in Java, which supports both SOCKS4
and SOCKS5 protocols. This software is distributed under GNU Lesser General Public
License, meaning that both binary and source code are freely available
and can be modified an distributed.
<p><font size='+0'>I would not bother you with long list of things I'm not<br>
responsible for. Let me just say, that you are using this program on your<br>
own risk, and it is not me to blame if anything doesn't work as you expected.<br>
I tried my best, but it is up to you to check if it works as you wish it<br>
to, the source code is there, so you can correct whatever you don't like.</font>
<h2>
Update Information</h2>
Current version is 1.01. Proxy have been rewised and there are some changes<br>
to the <a href='SOCKSLib.html'>Socks Library</a>. New features have been<br>
added to the proxy server itself, well at least one<br>
<ul>
<li>
Now it is possible to use this proxy from behind another proxy.</li>

<li>
Also proxy chaining is introduced, it allows you to configure the proxy<br>
to connect through a series of proxies before reaching the desired host:<br>
proxy1-> proxy2->...proxyN->desired_host. It is a strange feature but might<br>
be useful in some situations.</li>
</ul>
Some bug fixes have been done, it is now possible to use ICQ with this<br>
proxy server.<br>
<h2>
How to download</h2>
Source code pre compiled class files an documentation are all available<br>
for download. All of them are compressed using <tt>jar</tt> utility, which<br>
is part of the standard JDK distribution from SUN. The format is compatible<br>
with the one used by pkzip and Winzip programs, so you can use those programs<br>
to decompress these files.<br>
<br><a href='downloads/socks_bin.zip'>Pre<br>
compiled class files</a> - class files, configuration and batch files to<br>
run proxy server.<br>
<br><a href='downloads/socks_code.zip'>Source<br>
code </a>- Complete source code for SOCKS proxy and some other programs<br>
which use socks package.<br>
<br>
<br><a href='downloads/socks_docs.zip'>Socks<br>
documentation</a> - Documentation for socks package, for those who want<br>
to use it.<br>
<br><a href='docs/index.html'>Online Documentation</a> - Online version<br>
of the SOCKS documentation.<br>
<h2>
What this Server is good for?</h2>
Well, it is a not a commercial proxy server. It does not have plenty of<br>
features like address caching. Authentication scheme is rather simplistic,<br>
but can be extended, if you know how to program in Java. It is java application<br>
after all, which gives platform independence but at the cost of performance.<br>
But it is simple to install and use.<br>
<p>It is assumed that the socks library itself is more useful to most developers,<br>
rather than a simple server which uses the library. If you are a developer<br>
and want your applications to have support for SOCKSv5 protocol, you might<br>
find useful visiting <a href='SOCKSLib.html'>Socks Library</a> page.<br>
<h2>
SocksEcho</h2>

SocksEcho is another application which uses <tt>socks</tt> package. It<br>
is GUI echo client, which is SOCKS aware, you can make and accept connections<br>
through the proxy using this client. You can also send datagrams through<br>
SOCKS5 proxy. I have used it a lot for testing. This application is also<br>
included.<br>
<h2>
How to Install</h2>
First download pre compiled class files, and unzip the socks_bin.zip this<br>
will create a directory called socks. See README.html in this directory<br>
for further instructions.<br>
<h2>
Requirements</h2>
In order to run these application you will need Java Virtual Machine which<br>
supports Java 1.1 or higher. I have tested it with jdk1.1.6 and jdk1.2.2<br>
under Windows95 and on jdk1.1.5 under Solaris. Server application might<br>
be able to run even under java 1.0, but I haven't tested this.<br>
<br>&nbsp;<br>
<h2>Acknowledgments</h2>
I would like to thank people at <a href='http://sourceforge.net'>SourceForge<br>
<br>
</a> for the great services they provide to open source community.<br>&nbsp;<br>
