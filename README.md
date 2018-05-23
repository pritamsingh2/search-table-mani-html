<html>
	<head>
		<title>Search Table</title>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
		<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.6.1/jquery.min.js" type="text/javascript"></script>
		<script src="http://ajax.aspnetcdn.com/ajax/jquery.validate/1.9/jquery.validate.min.js" type="text/javascript"></script>
		<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
		<script src="js/form-validation.js"></script>
	</head>
	<style>
		body{
			border-style:double;
			border-color:black;
			background-color:white;
			border-width: thick;
			border-width: 3px;
		}
		.boxed {
			border: 1px solid black ;
			background-color:lightgrey;
			height: 150px;
			left:10px;
			margin: 3px;
		}
		.tab {
			overflow: hidden;
			background-color: black;
			border-top-left-radius: 5px;
			border-top-right-radius: 5px; 
			border-bottom-left-radius: 5px;
			border-bottom-right-radius: 5px; 
		}
		.tab button {
			background-color: grey;
			float: none;
			border-color:black;
			outline: none;
			cursor: pointer;
			padding: 15px 133px;
			transition: 0.9s;			
		}
		.tab button:hover {
			background-color: #ddd;
		}
		hr{
			border-color:grey;
		}
		#vertical{
			height: 320px;
			border-left: 3px solid black;
			position: absolute;
			top: 5px;
			left: 250px;
			text-align:center;
		}
		.boxed1 {
			border-top: 1px solid black ;
			background-color:lightyellow;
			height: 40px;
			left:5px;
			margin: 10px;
		}
		.previous {
			background-color: black;
			color: white;
			
		}

		.next {
			background-color: black;
			color: white;
		}
		#bar {
			text-decoration: none;
			display: inline-block;
			padding: 5px 10px;
		}
		.panel-primary {
			color: #333;
			background-color: lightyellow;
			border-color:black;
		}
		.nav{
			color: #333;
			background-color: blue;
			border-color:red;
		}
	</style>
	<body>
		<div class="container-fluid">
			<div class="row">
				<div class="panel panel-primary">
					<div class="row">
						<div class="col-sm-12">
							<ul class="nav nav-tabs nav-justified" style="background-color:lightgreen;">
								<li><a href="#"><i><b><font color="white" size="3px">All Books</font></b></i></a></li>
								<li><a href="#"><i><b><font color="black" size="3px">Books & E Books</font></b></i></a></li>
								<li><a href="#"><i><b><font color="white" size="3px">Magazine & Journals</font></b></i></a></li>
								<li><a href="#"><i><b><font color="white" size="3px">Media</font></b></i></a></li>
							  </ul>
						</div>
					</div>
					<br>
					<div class="row">
						<div class="col-sm-1">
						</div>
						<div class="col-sm-8">
							<input type="text" name="searchBar" placeholder="Search Content" style="background-color:lightgrey;width:950px;height:30px;border-color:grey;"/>
							&nbsp;&nbsp;&nbsp;&nbsp; 
						</div>
						<div class="col-sm-2">
						&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
						
							<button type="submit" class="searchButton" style="background-color:blue;width:100px;height:32px"><font color="white"><b>Search</b></font></button>
						</div>
					</div>
					<br>
					<div  class="row">
						<div class="col-sm-1">
						</div>
						<div class="col-sm-11">
							<u><a href="#">Advanced Search</a></u>
						</div>
					</div>
				</div>
			</div>
			<div class="row">
				<hr>
			</div>
			<div>
				<div class="row">
					<div class="col-sm-2">
						<font color="black" size="3px"><b>Search result</b></font>
					</div>
				</div>
				<br>
				<div class="row">
					<div class="col-sm-6 text-left">
						<a href="#" ><font color="blue">&laquo; Previous </font></a> |
						<a href="#" ><font color="blue">Next &raquo;</font></a>
					</div>
					<div class="col-sm-6 text-right">
						<select style="background-color:lightgrey">
							<option value="default">100 Per Page</option>
							<option value="150">150 Per Page</option>
							<option value="200">200 Per Page</option>
							<option value="250">250 Per Page</option>
							<option value="300">300 Per Page</option>

						</select >
						<select style="background-color:lightgrey">
							<option value="default">Sort</option>
							<option value="pageNo">Page wise</option>
							<option value="chapterName">Chapter wise</option>
						</select>
					</div>
				</div>
			</div>
			<div class="row">
				<div class="boxed1">
					<div class="col-sm-2 text-center">
					</div>
					<div class="col-sm-7 text-center">
						<font color="black" size="4px"><b>Description</b></font>
					</div>
					<div class="col-sm-2 text-right">
						<font color="black" size="4px"><b>Select</b></font>
					</div>
				</div>
			</div>
			<div class = "row">
				<div class="col-sm-2 text-center">
					<img src="https://media.wiley.com/product_data/coverImage300/30/04706591/0470659130.jpg" style="height:60px;width:60px;"/>
				</div>
				<div class="col-sm-7 text-left">
					<font color="black" size="3px"><b>1. <i>Handbook of Agricultural Entomology</i> by Helmut van Emden</b></font><br>
					<font color="black" size="3px"><b>Language: English</b></font><br>
					<font color="black" size="3px"><b>Publisher: New York: [Time-Life Books], [1969-1970]</b></font>
				</div>
				<div class="col-sm-2 text-right">
					<input type="checkbox" id= "checkBox1" style="height:20px;width:20px;">
				</div>
			</div><br>
			<div class = "row">
				<div class="col-sm-2 text-center">
					<img src="data:image/jpeg;base64,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"  style="height:60px;width:60px;"></img>
				</div>
				<div class="col-sm-7 text-left">
					<font color="black" size="3px"><b>2. <i>Wild about books </i> by Judy Sierra; Marc Tolon Brown</b></font><br>
					<font color="black" size="3px"><b>Language: English</b></font><br>
					<font color="black" size="3px"><b>Publisher: New York: Alfred A. Knopf, 2004.</b></font>
				</div>
				<div class="col-sm-2 text-right">
					<input type="checkbox" id= "checkBox2"style="height:20px;width:20px;">
				</div>
			</div><br>
			<div class = "row">
				<div class="col-sm-2 text-center">
					<img src="data:image/jpeg;base64,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"  style="height:60px;width:60px;"></img>
				</div>
				<div class="col-sm-7 text-left">
					<font color="black" size="3px"><b>3.<i> The purchase of books </i> by public libraries by Great Britain.</b></font><br>
					<font color="black" size="3px"><b>Language: English</b></font><br>
					<font color="black" size="3px"><b>Publisher: London, H.M. Stationery Off., 1972.</b></font>
				</div>
				<div class="col-sm-2 text-right">
					<input type="checkbox" id= "checkBox3" checked= "checked" style="height:20px;width:20px;"><br><br>
					<b><u><a href="#">Read</a>|<a href="#">Download</a></></b>
				</div>
			</div><br>	
			<div class = "row">			
				<div class="col-sm-11 text-right">
					<button type="submit" class="cancelButton" style="background-color:red;width:100px;height:30px"><font color="white"><b>Cancel</b></font></button>
					<button type="submit" class="reserveButton" style="background-color:blue;width:100px;height:30px"><font color="white"><b>Reserve</font></button>
				</div>
			</div>
			<div class="row">
				<div class="row">
					<div class="col-sm-2 text-center">
						<font color="black"><b>Speaker Notes</b></font>
					</div>
				</div>
				<br>
				<div class="row">
					<div class="col-sm-2 text-right">					
						<br><a href="#" id="bar" class="previous" data-slide="prev"><font size="5px"> 
							<span class="glyphicon glyphicon-chevron-left"></span></font></a>
					</div>

					<div class="col-sm-2 ">
						<img src="https://3.bp.blogspot.com/-nWFQOMITbsQ/TaUlwWMqRtI/AAAAAAAAAfA/uXiFqh69Wzw/s80/sunrise.png"  style="height:60px;width:40%;"></img>
						<u><font color="black"><i> "Handbook of Agricultural Entomology" </i>by Helmut van Emden is a landmark publication for students</b></font></u>
					</div>

					<div class="col-sm-3 ">
						<img src="http://digital-storytime.com//graphics/DS_Logo.png"  style="height:60px;width:60%;"></img>
						<u><font color="black"><b>"This whimsical storyline is one that kids will love and identify with too, since young children are often as hard on their books as any monkey in the zoo!"</b></font></u>
					</div>
					
					<div class="col-sm-2 ">
						<img src="https://www.scribendi.com/images/cms/thumbnails/How-to-Write-a-Report-on-a-Book_100x100.jpg"  style="height:60px;width:60%;"></img>
						<u><font color="black"><b>"Historical fiction is mostly smoke and mirrors"</b></font></u>
					</div>

					<div class="col-sm-2 text-left">
						<br><a href="#" id="bar" class="next" data-slide="next"><font size="5px">
						<span class="glyphicon glyphicon-chevron-right"></span></font></a>
					</div>
				</div>
			</div>
		</div>
	</body>
</html>
