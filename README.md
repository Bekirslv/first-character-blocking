# first-character-blocking
prevent entering 0 for the first character
//Jquery 





$('#number').keypress(function (e) {
    if (this.value.length == 0 && e.which == 48)
        {
            $(this).next().show();
          return false;
        }
           else{
               $(this).next().hide();
           }
        });
