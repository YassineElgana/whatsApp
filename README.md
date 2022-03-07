# whatsApp

 function send_handle(){

/*let num=document.getElementById("number").value;
console.log(num)

  let name= document.getElementById("name").value;

var win = window.open(`https://wa.me/${num}?text=${name}`, '_blank');*/


  var divToPrint=document.getElementById('print');

  var newWin=window.open('','Print-Window');

  newWin.document.open();

  newWin.document.write('<html><head><link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.3.1/dist/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous"></head><body onload="window.print()">'+divToPrint.innerHTML+'</body></html>');

  newWin.document.close();
  
  setTimeout(function(){newWin.close();},10);


 
    }
