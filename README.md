# node WiFiScanner

Node WiFiScanner is a nodejs module that uses the OS utility to scan WiFi access
points.

On Mac, it will use the `airport` command.
On Linux, il will use `iwlist` command.

How to use :

	// scanner.js

	var wifiscanner = require('./wifiscanner.js');

	wifiscanner.scan(function(err, data){
		if (err) {
			console.log("Error : " + err);
			return;
		}

		console.log(data);
	});
	
Scanning surrounding WiFi access points is usefull for getting geolocation. See `geolocation.js` for an example.

## Author

* Maurice Svay <maurice@svay.com>, [http://svay.com](http://svay.com)

## Simplified BSD License

	Copyright 2012 Maurice Svay. All rights reserved.

	Redistribution and use in source and binary forms, with or without modification, are
	permitted provided that the following conditions are met:

	   1. Redistributions of source code must retain the above copyright notice, this list of
	      conditions and the following disclaimer.

	   2. Redistributions in binary form must reproduce the above copyright notice, this list
	      of conditions and the following disclaimer in the documentation and/or other materials
	      provided with the distribution.

	THIS SOFTWARE IS PROVIDED BY Maurice Svay ''AS IS'' AND ANY EXPRESS OR IMPLIED
	WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
	FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL Maurice Svay OR
	CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
	CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
	SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
	ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
	NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
	ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

	The views and conclusions contained in the software and documentation are those of the
	authors and should not be interpreted as representing official policies, either expressed
	or implied, of Maurice Svay.