# HC_Room_AV
Sacramento Stake HC Room AV Setup


http://192.168.0.120/aj.html?a=rout
http://192.168.0.120/aj.html?a=input
http://192.168.0.120/aj.html?a=outp  /*Get Output Information

http://192.168.0.120/aj.html?a=stat
http://192.168.0.120/aj.html?a=devi

http://192.168.0.120/aj.html?a=command&cmd=A&p1=0 /*No Source to Output 1
http://192.168.0.120/aj.html?a=command&cmd=A&p1=1 /*Input 1 to Output 1
http://192.168.0.120/aj.html?a=command&cmd=A&p1=2 /*Input 2 to Output 1
http://192.168.0.120/aj.html?a=command&cmd=A&p1=3 /*Input 3 to Output 1
http://192.168.0.120/aj.html?a=command&cmd=A&p1=4 /*Input 4 to Output 1

http://192.168.0.120/aj.html?a=command&cmd=B&p1=0 /* No Source to Output 2
http://192.168.0.120/aj.html?a=command&cmd=B&p1=0 /* Input 1 to Output 2
http://192.168.0.120/aj.html?a=command&cmd=B&p1=0 /* Input 2 to Output 2
http://192.168.0.120/aj.html?a=command&cmd=B&p1=0 /* Input 3 to Output 2
http://192.168.0.120/aj.html?a=command&cmd=B&p1=0 /* Input 4 to Output 2

  <script>
      var xhr = new XMLHttpRequest();

      function getHttp(){
        
        xhr.onreadystatechange = function() {
          if (xhr.readyState == XMLHttpRequest.DONE) {
            var values = JSON.parse(xhr.responseText);
            alert(xhr.responseText);
            console.log(values);
          }
        }
        xhr.open("GET", "https://api.ncbi.nlm.nih.gov/datasets/v2alpha/gene/id/59067");
        xhr.send();
      };
    </script>
  </head>

  <body>
    <div class="container">

      <div class="page-header">
        <h1>Bootstrap grid examples</h1>
        <p class="lead">Basic grid layouts to get you familiar with building within the Bootstrap grid system.</p>
        <button id="test" onclick="getHttp()">Test Button</button>
      </div>

    </div> <!-- /container -->
  </body>
