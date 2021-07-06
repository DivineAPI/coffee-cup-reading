
#################################
Coffee Cup Reading - DivineAPI
#################################
Start your FREE Trial to get your API KEY,  `https://divineapi.com <https://divineapi.com>`_

|travis| |Docs| |Maintenance yes| |SayThanks| |Paypal|
    
    
.. image:: https://divineapi.com/assets/images/logo.svg
   :height: 412px
   :width: 898px
   :alt: divineapi logo
   :align: center


What is Coffee Cup Reading API?
==============
The developers are provided with an exceptional opportunity of adding Coffee cup Reading
API to their applications designed by the Divine API that retrieves data about all zodiac signs
for today, yesterday and tomorrow, tarot related APIs and much more.

..
  Feel free to contribute on `Github <http://github.com/divineapi/horoscope-api>`_.




Why Coffee Cup Reading API?
==========
The Divine API can benefit the developers by adding the Coffee cup reading API to their
application and give their users an amazing chance to interpret the patterns of their coffee
residuals at the bottom of the cup.



Features
==========

- Horoscope API tells you about your profession in a given day.
- It provides the users with health tips depending on their zodiac signs.
- People will get to know what would their emotions bring to the surface.
- Travel horoscope is an amazing feature provided to the user.
- It gives all the users cosmic tips, tips to singles and couples.


Benefits
==========

- It will tell you how your day is going to be.
- The Horoscope API display what color and numbers are lucky for you in a given day.
- Knowing that stars are in preferred position will help your confidence blossom.


URL
===
.. code-block:: python

    POST: https://divineapi.com/api/1.0/get_coffee_cup_reading.php


Parameters
==========

api_key : 
   Your API  KEY.


Result Example:
=====
.. code-block:: json

    {
        "success": 1,
        "message": "Coffee Cup Reading result.",
        "data": {
            "prediction": {
                "present_title": "present",
                "present_image": "image_url",
                "present_content": "present content",
                "near_future_title": "Near Future",
                "near_future_image": "image_url",
                "near_future_content": "Near Future content",
                "distant_future_title": "Distant Future",
                "distant_future_image": "image_url",
                "distant_future_content": "Distant Future content"
            }
        }
    } 


Example 
=======



cURL
^^^^
.. code-block:: curl

    curl -d "api_key=YOUR_API_KEY" -X POST https://divineapi.com/api/1.0/get_coffee_cup_reading.php


Python
^^^^^^
.. code-block:: python

   import requests
   from requests.structures import CaseInsensitiveDict

   url = "https://divineapi.com/api/1.0/get_coffee_cup_reading.php"

   headers = CaseInsensitiveDict()
   headers["Content-Type"] = "application/x-www-form-urlencoded"

   data = "api_key=YOUR_API_KEY"


   resp = requests.post(url, headers=headers, data=data)

   print(resp.status_code)


Javascript
^^^^^^^
.. code-block:: javascript

   var url = "https://divineapi.com/api/1.0/get_coffee_cup_reading.php";

   var xhr = new XMLHttpRequest();
   xhr.open("POST", url);

   xhr.setRequestHeader("Content-Type", "application/x-www-form-urlencoded");

   xhr.onreadystatechange = function () {
      if (xhr.readyState === 4) {
         console.log(xhr.status);
         console.log(xhr.responseText);
      }};

   var data = "api_key=YOUR_API_KEY";

   xhr.send(data);


PHP
^^^
.. code-block:: php

   <?php
    $url = "https://divineapi.com/api/1.0/get_coffee_cup_reading.php";

    $curl = curl_init($url);
    curl_setopt($curl, CURLOPT_URL, $url);
    curl_setopt($curl, CURLOPT_POST, true);
    curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);

    $headers = array(
       "Content-Type: application/x-www-form-urlencoded",
    );
    curl_setopt($curl, CURLOPT_HTTPHEADER, $headers);

    $data = "api_key=YOUR_API_KEY";

    curl_setopt($curl, CURLOPT_POSTFIELDS, $data);

    $resp = curl_exec($curl);
    curl_close($curl);
    var_dump($resp);
   ?>
    
    
jQuery Ajax
^^^^^^
.. code-block:: javascript

    $.ajax({
   type:'POST',
   url:'https://divineapi.com/api/1.0/get_coffee_cup_reading.php',
   data: {api_key:'YOUR_API_KEY'},
   success:function(data){
   console.log(data);
   }
    });


ECMAScript (ES6)
^^^^^^
.. code-block:: javascript

    const URL = 'https://divineapi.com/api/1.0/get_coffee_cup_reading.php?api_key=YOUR_API_KEY';
    fetch(URL, {
        method: 'POST'
    })
    .then(response => response.json())
    .then(json => {
        const date = json.current_date;
        console.log(date);
    });


Services
========
|Horoscope| |Daily Tarot| |Yes No Tarot| |Fortune Cookie| |Coffee Cup|



License
=======

2021 Divine API

Licensed under the Apache License, Version 2.0 (the "License");

    http://www.apache.org/licenses/LICENSE-2.0



Contact
=======

Questions? Suggestions? Feel free to contact me at admin@divineapi.com


Credits
=======

"DivineAPI" was created by `Azhar <https://azhar-spiderdev.github.io/portfolio>`_

Source of updates - https://divineapi.com/coffee-cup-reading-api

Please feel free to use and adapt this awesome API.

    
.. |Travis| image:: https://img.shields.io/badge/7%20Days%20Free%20trial-%23039BE5.svg?&style=for-the-badge&logoColor=white
    :target: https://divineapi.com/register

.. |SayThanks| image:: https://img.shields.io/badge/API%20Documentation-FCC624?style=for-the-badge&logoColor=white
    :target: https://divineapi.com/api-doc

.. |Paypal| image:: https://img.shields.io/badge/Other%20Services-%2311AB00.svg?&style=for-the-badge&logoColor=white
    :target: `Services`_
    
.. |Horoscope| image:: https://img.shields.io/badge/Daily%20Horoscope-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/horoscope-api


.. |Daily Tarot| image:: https://img.shields.io/badge/Daily%20Tarot-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/daily-tarot
    
    
.. |Yes No Tarot| image:: https://img.shields.io/badge/Yes%20Or%20No%20Tarot-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/yes-or-no-tarot
    
.. |Fortune Cookie| image:: https://img.shields.io/badge/Fortune%20Cookie-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/fortune-cookie
    
.. |Coffee Cup| image:: https://img.shields.io/badge/Coffee%20Cup-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/coffee-cup-reading


.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`modindex`
.. * :ref:`search`
