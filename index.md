<body>
	
	<style>
		
		iframe {
		    border: 1px solid black;
		    width: 100%;
		    height: 500px;
		    box-shadow: 0px 5px 15px Black;
		}

		input {
		    width: 80%;
		    color: Black;
		    background-color: White;
		    border: 1px solid Black;
		    box-shadow: 0px 5px 15px Black;
		    border-radius: 5px;
		    margin-left: 15px;
		}

		button {
		    color: black;
		    background-color: white;
		    border: 1px solid Black;
		    box-shadow: 0px 5px 15px Black;
		    border-radius: 5px;
		}
	</style>

	<p><input id="inweb" value="https://google.fr">
   
	<button id="go" onclick="goWeb()">Aller</button></p><p>Resultat:</p>

	<iframe id="outweb"
	    width="300"
	    height="200"
	    allow="fullscreen"
	    src="https://fr.wikipedia.org/wiki/Robert_Louis_Stevenson">
	</iframe>
	<script>
		var iframe = document.querySelector('#outweb');
		var input = document.querySelector('#inweb');
		var button = document.querySelector('#go');
		function goWeb(){
			iframe.src = input.value;
		}
	</script>
</body>
