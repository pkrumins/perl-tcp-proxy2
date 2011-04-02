This is a simple TCP proxy written in Perl that uses IO::Socket::INET and
IO::Select abstractions to create an evented (asynchronous, on select() call
based) server.

It was written by Peteris Krumins (peter@catonmat.net).
His blog is at http://www.catonmat.net  --  good coders code, great reuse.

I modified the proxy that I had written for my "Turn any Linux computer into
SOCKS5 proxy in one command" article:

    http://www.catonmat.net/blog/linux-socks5-proxy

And wrote another article:

    http://catonmat.net/blog/perl-tcp-proxy

------------------------------------------------------------------------------

Here is how it works:

    $ ./tcp-proxy2.pl <local port> <host:port>

This command proxies all tcp connections to <local port> to <host:port>.

------------------------------------------------------------------------------

Happy proxying!

Sincerely,
Peteris Krumins
http://www.catonmat.net
