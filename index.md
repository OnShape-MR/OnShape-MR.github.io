<b> What is Onshape for Mixed Reality project?

<iframe width="560" height="315" src="https://www.youtube.com/embed/myeTj3Bg80Q?rel=0&cc_load_policy=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe><br>

[Download or clone the project ;)](https://github.com/OnShape-MR/Onshape-For-Mixed-Reality)


<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>

<script>
$( document ).ready(function() {

var port = 1212;
var hololensA = "hololens-roe52";
var hololensB = "hololens-5cofq";

var url = new URL(window.location.href);

var code = url.searchParams.get("code");

    $("#localhost").attr("href", "http://localhost:"+port+"/?code=" + code);
    $("#HololensA").attr("href", "http://"+hololensA+":"+port+"/?code=" + code);
    $("#HololensB").attr("href", "http://"+hololensB+":"+port+"/?code=" + code);
	
	$("#Code").text(code);
});

</script>


## 1. Se connecter

<a href="https://oauth.onshape.com/oauth/authorize?response_type=code&client_id=4OMIXKUICROTVQSOOGSBGM2YLE5KVHI2ADZ3IHY=&grant_type=authorization_code&redirect_uri=https://Rufus31415.github.io/">Obtenir un token</a>


## 2. Transmettre le token

Token : <b id="Code"></b><br><br>
<a href="" id="localhost">Local</a><br><br>
<a href="" id="HololensA">HololensA</a><br><br>
<a href="" id="HololensB">HololensB</a>
