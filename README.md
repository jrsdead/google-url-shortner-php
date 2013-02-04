google-url-shortner-php
=======================

PHP class for using the Google url shortener

## Usage:
	<?php
	require_once 'googleurlshortener.php';
	
	// Shorten an URL.
	$longurl = 'http://www.google.com';
	if ($shorturl = googleurlshortener::shortenurl($longurl)) {
		echo $longurl . ' shortened: ' . $shorturl . '<br>';
	}
	$shorturl = 'http://goo.gl/CyLE'; // (http://www.github.com)
	if ($longurl = googleurlshortener::expandURL($shorturl)) {
		echo $shorturl . ' expanded: ' . $longurl . '<br>';
	}