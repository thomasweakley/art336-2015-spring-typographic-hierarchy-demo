		Web Typography

		Web typography refers to the use of fonts on the World Wide Web. When HTML was first created, font faces and styles were controlled exclusively by the settings of each Web browser. There was no mechanism for individual Web pages to control font display until Netscape introduced the <font> tag in 1995, which was then standardized in the HTML 2 specification. However, the font specified by the tag had to be installed on the user's computer or a fallback font, such as a browser's default sans-serif or monospace font, would be used. The first Cascading Style Sheets specification was published in 1996 and provided the same capabilities.
		
		Being a web designer will soon require a deeper understanding of typography and how typefaces work. As we move in this direction, our options may be limited at first, but the pool of choices will steadily grow. And as we know, with great power comes great responsibility. Just because you can use the font that looks like it’s wearing bellbottoms, doesn’t mean you should.
		
		Jason Santa Maria
		
		The CSS2 specification was released in 1998 and attempted to improve the font selection process by adding font matching, synthesis and download. These techniques did not gain much use, and were removed in the CSS2.1 specification. However, Internet Explorer added support for the font downloading feature in version 4.0, released in 1997. Font downloading was later included in the CSS3 fonts module, and has since been implemented in Safari 3.1, Opera 10 and Mozilla Firefox 3.5. This has subsequently increased interest in Web typography, as well as the usage of font downloading.
		
		CSS1
		
		In the first CSS specification, authors specified font characteristics via a series of properties:
		
		font-family
		font-style
		font-variant
		font-weight
		font-size
		
		All fonts were identified solely by name. Beyond the properties mentioned above, designers had no way to style fonts, and no mechanism existed to select fonts not present on the client system.
		
		Web-Safe Fonts
		
		Web-safe fonts are fonts likely to be present on a wide range of computer systems, and used by Web content authors to increase the likelihood that content displays in their chosen font. If a visitor to a Web site does not have the specified font, their browser tries to select a similar alternative, based on the author-specified fallback fonts and generic families or it uses font substitution defined in the visitor's operating system.
		
		Generic Font Families
		
		To give Web designers some control over the appearance of fonts on their Web pages, even when the specified fonts are not available, the CSS specification allows the use of several generic font families. These families are designed to split fonts into several categories based on their general appearance. They are commonly specified as the last in a series of fallback fonts, as a last resort in the event that none of the fonts specified by the author are available. There are five generic families:
		
		Sans-serif
		Fonts that do not have decorative markings, or serifs, on their letters. These fonts are often considered easier to read on screens.
		
		Serif
		Fonts that have decorative markings, or serifs, present on their characters.
		
		Monospace
		Fonts in which all characters are equally wide.
		
		Cursive
		Fonts that resemble cursive writing. These fonts may have a decorative appearance, but they can be difficult to read at small sizes, so they are generally used sparingly.
		
		Fantasy
		Fonts that may contain symbols or other decorative properties, but still represent the specified character.
		
		WEB FONTS
		
		History
		
		A technique to download remote fonts was first specified in the CSS2 specification, which introduced the @font-face rule.
		
		It was (and remains) controversial because using a remote font as part of a Web page allows the font to be freely downloaded. This could result in fonts being used against the terms of their license or illegally spread through the Web. TrueDoc (PFR), Embedded OpenType (EOT) and Web Open Font Format (WOFF) are formats designed to address these issues.
		
		Since the introduction of Internet Explorer 4, font embedding employing EOT has been used mainly for displaying characters in writing systems that are not supported by default fonts. Use on English-language Web sites was virtually non-existent. With the releases of Firefox 3.5, Opera 10 and Safari 3.1, usage employing other formats is expected to increase.
		
		File Formats
		
		By using a specific CSS @font-face embedding technique it is possible to embed fonts such that they work with IE4+, Firefox 3.5+, Safari 3.1+, Opera 10+ and Chrome 4.0+. This allows the vast majority of Web users to access this functionality. Some commercial foundries object to the redistribution of their fonts. For example, Hoefler & Frere-Jones says that, while they “...enthusiastically [support] the emergence of a more expressive Web in which designers can safely and reliably use high-quality fonts online,” the current delivery of fonts using @font-face is considered “illegal distribution” by the foundry and is not permitted.
		
		Naturally this does not interfere with fonts and foundries under free licenses.
		
		TrueDoc
		Bitstream developed TrueDoc, the first standard for embedding fonts. TrueDoc was natively supported in Netscape Navigator 4, but was discontinued in Netscape Navigator 6 and Mozilla, because Netscape could not release Bitstream's source code. A WebFont Player plugin was available for Internet Explorer, but the technology had to compete against Microsoft’s Embedded OpenType fonts, natively supported since version 4.0.
		
		Embedded OpenType
		Internet Explorer has supported font embedding through the proprietary Embedded OpenType standard since version 4.0. It uses digital rights management techniques to help prevent fonts from being copied and used without a license. A simplified subset of EOT has been formalized under the name of CWT Compatibility Web Type, formerly EOT-Lite
		
		Scalable Vector Graphics
		Web typography applies to SVG in two ways:
		
		All versions of the SVG 1.1 specification, including the SVGT subset, define a font module allowing the creation of fonts within an SVG document. Safari introduced support for many of these properties in version 3. Opera added preliminary support in version 8.0, with support for more properties in 9.0.
		The SVG specification lets CSS apply to SVG documents in a similar manner to HTML documents, and the @font-face rule can be applied to text in SVG documents. Opera added support for this in version 10, and WebKit since version 325 also supports this method using SVG fonts only.
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		
		TrueType/OpenType
		Linking to industry-standard TrueType (TTF) and OpenType (TTF/OTF) fonts are supported by Mozilla Firefox 3.5+, Opera 10+, Safari 3.1+, Google Chrome 4.0+. Internet Explorer 9+ supports only those fonts with embedding permissions set to installable.
		
		Web Open Font Format
		WOFF has been supported by Mozilla Firefox 3.6+, Google Chrome 5+, Opera Presto, and is supported by Internet Explorer 9 (since March 14, 2011). Support is available on Mac OS X Lion's Safari from release 5.1.
		
		An example of a CSS @font-face setup:
		@font-face { font-family: 'Journal'; src:url('http://your-own.site/fonts/journal/journal.woff') format('woff'), url('http://your-own.site/fonts/journal/journal.svg#Journal') format('svg'), url('http://your-own.site/fonts/journal/journal.ttf') format('truetype'), url('http://your-own.site/fonts/journal/journal.eot'), url('http://your-own.site/fonts/journal/journal.eot?#iefix') format('embedded-opentype'); font-weight: normal; font-style: normal; }
		
		Lorem Ipsum Dolor Sit Amet Consectetur
		Lorem Ipsum Dolor Sit Amet Consectetur
		Lorem Ipsum Dolor Sit Amet Consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin rhoncus metus at tempus gravida. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Mauris mollis orci sit amet turpis porttitor, a molestie enim viverra.
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur
		Lorem ipsum dolor sit amet consectetur