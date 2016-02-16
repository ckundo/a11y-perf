## Accessibility Testing Library Performance

This is a test page to benchmark performance of [Deque's aXe-core](https://github.com/dequelabs/axe-core), 
[Google's Accessibility Developer Tools](https://github.com/googlechrome/accessibility-developer-tools),
and [SquizLabs HTML CodeSniffer](https://github.com/squizlabs/HTML_CodeSniffer).

When run in Firefox 44.0.2 against the page, the libraries performed thusly:

- Accessibilty Developer Tools: 618.7599999999984 milliseconds
- HTML Code Sniffer: 274.5199999999995 milliseconds
- aXe 931.7999999999302 milliseconds

It's hard to draw meaningful performance comparisons amongst accessibility
testing libraries, since the coverage and types of tests vary widely amongst
them. At the very least we can see that on a complex page any of these libraries
will bring the framerate to 0 for at least a couple hundred milliseconds.

The markup and content used for the performance timings comes from
http://www.html5accessibility.com/html5elements/, created by @ackernaut and
@ThePacielloGroup
