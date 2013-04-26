
aciFragment - Store/read URL fragment variables

Features:

- possibility of storing/reading variables from the fragment section of a URL
  (the value following the first # found in the URL);

- the keys/values are automatically encoded/decoded and the URL is changed to
  preserve the value of the anchor (if any);

- aciFragment provides a method that can be called from within the
  onclick event handler for the links that link to an anchor.

Simple usage:

$(function(){

    $(document).aciFragment();

    var api = $(document).aciFragment('api');

    $('a').click(function() {
        api.click($(this));
        return false;
    });

});

aciFragment jQuery Plugin v1.1.0
http://acoderinsights.ro

Copyright (c) 2013 Dragos Ursu
Dual licensed under the MIT or GPL Version 2 licenses.

Require jQuery Library >= v1.7.1 http://jquery.com
+ aciPlugin >= v1.1.1 https://github.com/dragosu/jquery-aciPlugin

Date: Apr Fri 26 18:00 2013 +0200
