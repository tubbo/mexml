# MeXML: Message eXchange Markup Language

## what is it?

MeXML is a language for describing e-mail messages, based on [XML](http://www.w3.org/XML/) and designed for web application development. MeXML makes it easy to generate templates for e-mails the way you see them, even including XHTML 1.0 formatting elements in the DOCTYPE. In fact, MeXML files behave exactly like HTML files only with different headers!

## examples

an example message is provided in this repo ("example.mex") that shows off all of MeXML's features, but here's a short one just to show how easy and beautiful it is to create e-mails with MeXML!

	<?xml version="1.0" xmlns="http://psychedeli.ca/code/mexml" xml:lang="en" ?>
	<message>
		<head>
			<from href="tha_dark_lord@mordor.co.uk">Sauron</from>
			<to href="elves@middle.earth.net">The Elves</to>
			<to href="dwarves@middle.earth.net" type="cc">The Dwarves</to>
			<to href="men@middle.earth.net" type="cc">The Men</to>
			<to href="morgoth@middle.earth.net" type="bcc">Morgoth</to>
			<subject>haha kiss the rings bitch!!!</subject>
		</head>
		<body>
			<p>
				I done got all yo rings. Have fun in your boats bitchezzz!!!
			</p>
		</body>
	</message>

## rendering

MeXML will include parsers for various languages, including Ruby, Python and PHP. It is geared towards web development and thus is focused primarily on languages which support a "web application framework":http://en.wikipedia.org/Web_Application_Framework.