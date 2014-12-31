$('#build').click(function(){
	console.log("Build Clicked");
	
	if(Modernizr.localstorage){
		allVals =[];
		$("input:checked").each(function(){
			console.log($(this).attr('name'));
			console.log($(this).val());
			allVals.push([$(this).attr('name'),parseInt($(this).val())]);
		});
		
		console.log(JSON.stringify(allVals));
		localStorage.setItem("toppings",JSON.stringify(allVals));
		$(location).attr('href','pizzachart.html');
	}
	else {
		alert("The browser does not support localStorage");
	}
	
});