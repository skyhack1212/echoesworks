[![Build Status](https://travis-ci.org/phodal/echoesworks.svg?branch=master)](https://travis-ci.org/phodal/echoesworks)
[![Version](http://img.shields.io/npm/v/echoesworks.svg?style=flat)](http://http://img.shields.io/npm/v/echoesworks.svg)
[![Code Climate](https://codeclimate.com/github/phodal/echoesworks/badges/gpa.svg)](https://codeclimate.com/github/phodal/echoesworks)
[![Test Coverage](https://codeclimate.com/github/phodal/echoesworks/badges/coverage.svg)](https://codeclimate.com/github/phodal/echoesworks)
[![Node](https://img.shields.io/node/v/gh-badges.svg?style=flat)]()
[![npm](https://img.shields.io/npm/dm/echoesworks.svg?style=flat)]()
[![Bower](https://img.shields.io/bower/v/echoesworks.svg?style=flat)]()
[![LICENSE](https://img.shields.io/badge/license-MIT-green.svg?style=flat)]()

#[EchoesWorks](http://www.echoesworks.com/)#

> Next-Generation Tech Blog/Presentation Framework

zh

> 下一代技术``博客``/``展示``框架
 
Online Demo: [http://demo.echoesworks.com/](http://demo.echoesworks.com/) 
 
##Feature

###Core

- ``Markdown`` Presentation
- Integrate Github Code/Gist Code
- ``Full Screen`` Background Image
- Left/Right Images Support
- Process Bar

###Addon

- Timer Audio
- Timer subtitles
- Time Control

##Usage##


1.Install

    bower install echoesworks
    
2.Data

create ``example.md`` & ``data.json`` under ``data`` folder 
    
- Markdown Slide
- Data for code & Time Control     
    
3.Code    

     var EW = new EchoesWorks({
     		element: 'slide'
     	});

Example with slide

		EchoesWorks.get('data/example.md', function(data){
				document.querySelector('slide').innerHTML = EchoesWorks.md.parse(data);
				EchoesWorks.imageHandler();
				new EchoesWorks({
					element: 'slide'
				});
			})


##Setup Development##

1.Install devDependencies

     npm install

2.Development

3.Run Test

     npm test
      
4.Push Code & Waiting CI            

##Inspired by & Thanks to##

- Slide

    * [https://github.com/markdalgleish/bespoke.js](https://github.com/markdalgleish/bespoke.js)
    * [https://github.com/bartaz/impress.js](https://github.com/bartaz/impress.js)

- Markdown
    
    * [https://github.com/simonwaldherr/micromarkdown.js/](https://github.com/simonwaldherr/micromarkdown.js/)

- Time 
    
    * [https://github.com/vorg/timeline.js](https://github.com/vorg/timeline.js)

- Process Bar 
 
    * [https://github.com/jacoborus/nanobar](https://github.com/jacoborus/nanobar)

##License##

MIT. See `LICENSE.txt` in this directory.

