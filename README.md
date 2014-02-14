2
=

Assignment 2 AST
var data = { 
Students : [
	{ name : "Sander", Studentnumber: "1000678" },
	{ name : "Jonne-Marie", Studentnumber: "1000879" },
	{ name : "Joop", Studentnumber: "12345786" },
	{ name : "Jan", Studentnumber: "1098263" },
	{ name : "Tim", Studentnumber: "11297310" }
	],
Assignments : [
	{ Number: "1", description : "Alternatives" }, 
	{ Number: "2", description: "Add Assignments and Students" },
	{ Number: "3", description: "Dance" },
	{ Number: "4", description: "Sing" },
	{ Number: "5", description: "Jump around" }
	]
};
var rawHtml =  "<h2>Students</h2><ul> {{#Students}} <li>{{name}} - {{Studentnumber}} </li> {{/Students}} </ul> <h2>Assignments</h2><ul> {{#Assignments}} <li>{{Number}} - {{description}}</li> {{/Assignments}} </ul>";
	var template = Handlebars.compile(rawHtml);
	var html = template(data);
	$(".session3").append(html);
	
