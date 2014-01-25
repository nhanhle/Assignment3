Assignment3
===========
<!doctype html>
<html>
<head>
	<title>Assingment#3-Around The Wourld</title>
	<meta charset=utf8>
</head>
<body>
	THIS SPACE INTENTIONALLY LEFT BLANK.
<script src="http://thomaswilburn.net/sccc/data/expenditures.js"></script>
<script>	
	var highest = {amount: 0};	 
	for (var i = 0; i < expenditures.length; i ++) {
	var Amoun = expenditures[i];
		if (Amoun.amount > highest.amount) {
		highest = Amoun;
		} 
	}
	var lowest = {amount : highest};
	for (var i = 0; i < expenditures.length; i ++) {
	var Amounn = expenditures[i];
		if (Amounn.amount < lowest.amount) {
		lowest = Amounn;
		} 
	}
	
	average = (parseFloat(highest.amount) + parseFloat(lowest.amount)) / 2;
	console.log("Highest expenditures: " + '"' + highest.country ,
					' " ' + " with " + highest.amount + "  GDP.");
	console.log("Lowestest expenditures: " + '"' + lowest.country ,
					' " ' + " with " + lowest.amount + "  GDP.");
	console.log("Average expenditures: " + average + " GDP.");
	
</script>
</body>
</html>
