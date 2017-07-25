# send-display-value-using-ajax

In this git repository you can see and learn how to send and display data of text box on button click using ajax without page refresh

below code is for getting value of text box using id

var val1 = $('#term').val();

below code is for sending and display value using ajax

$.ajax({

      type: "POST",

      url: "search.php",

      data: {val1:val1},

      cache: false,

      success: function(html)

      { 

           $("#result").html(html).show();

      }
                        
});
