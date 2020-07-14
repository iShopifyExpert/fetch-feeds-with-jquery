# fetch-feeds-with-jquery

   
   
   <div id="all-sign"></div>
   <script src="http://code.jquery.com/jquery-1.11.0.js"></script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.8.4/moment.min.js"></script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-rss/3.3.0/jquery.rss.min.js"></script>
   <script>
   jQuery(function($) {
    $("#all-sign").rss("http://horoscopeservices.co.uk/daily_delivery/feed.asp?uid=781398952", {
      entryTemplate: '<li>[{date}]<br/>{title}<br/>{shortBodyPlain}</li>',
      dateFormat: "ddd, Do MMMM, YYYY, h:mm:ss a",
      limit: 12,
     });
   });
   </script>
   <style>
   #all-sign ul {
    margin: 0;
    padding: 0;
    display: block;
    text-align: center;
    list-style: none;
}
#all-sign ul li {
    margin: 20px 0 10px;
    padding: 0 10px;
    display: inline-block;
    max-width: 280px;
    vertical-align: top;
}
#all-sign li small {
    display: block;
    text-decoration: underline;
}
#all-sign ul li .sign-title {
    font-size: 18px;
    font-weight: bold;
    display: block;
    margin: 5px 0;
}
#all-sign ul li .sign-description {
    display: block;
    margin: 15px 0;
}
#all-sign ul li img:hover {
    filter: grayscale(1);
   }
    </style>
