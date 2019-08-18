---
---

<!DOCTYPE html>
<html>
	<head>
		<title>{{ page.student }} | Project Report </title>
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
        <link rel="stylesheet" href="resources/style.css">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/0.100.1/css/materialize.min.css">
        <link rel="stylesheet" href="https://rawgit.com/coala/coalaCSS/master/coala.css">
        <script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/0.100.1/js/materialize.min.js"></script>
        <link href="https://fonts.googleapis.com/css?family=Roboto+Mono:300,300i,400,400i,700,700i|Roboto:100,200,300,400,500,600,700,800,900|Ubuntu+Mono|Overpass+Mono|Inconsolata" rel="stylesheet">
        <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
        <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
	</head>
	<body class='report'>
		<div class="container">
        <br>
            <div class="row no-margin">
                <div class="col m12">
                    <h4 class="left light">Google Summer of Code 2019 Work Product Submission </h4>
                </div>
                <br>
            </div> 
            <br>
            <div class="row no-margin">
                <div class="col m6">
                    <div class="card flex1">
                        <div class="card-content">
                            <h5 class="light no-margin"><a href="{{page.organisation_link}}"><h4>{{ page.organisation }}</h4></a></h5>
                            <h3 class="light">{{ page.student }}</h3>
                            <p>{{page.bio | markdownify}}</p>
                        </div>
                    </div>
                </div>
                <div class="col m3">
                    <div class="card flex1">
                        <div class="card-content">
                            <div class="center"><h4 class="light no-margin">Project Title</h4></div>
                            <br>
                            <div class="center"><a href="{{page.project_link}}"><h3>{{ page.project }}</h3></a></div>
                        </div>
                    </div>
                    <div class="card flex1">
                        <div class="card-content">
                        <div class="center"><h5 class="light no-margin">Mentors</h5></div>
                        <br>
                        <div class="center"><h4>{{ page.mentors  | markdownify }}</h4></div>
                        </div>
                    </div>
                </div>
                <div class="col m3">
                    <div class="card flex1">
                        <div class="card-content links-section">
                            {% for ih in page.social %}
                                <div class="link">
                                {% for item in ih %}
                                    <div class="row no-margin ">
                                        <div class="col m4"><h5>{{item[0]}}</h5></div>
                                        <div class="col m8"><a href="{{item[1][1]['link']}}"><h5>{{item[1][0]['username']}}</h5></a></div>
                                    </div>
                                    <br>
                                    <br>
                                    <br>
                                {% endfor %}
                                </div>
                            {% endfor %}
                            <div class="row no-margin center">
                                <div class="col m12"><i class="fa fa-envelope-o"></i></div>
                                <br>
                                <div class="col m12"><h6><a href="mailto:agrawal.arpit14@gmail.com">{{ page.email }}</a></h6></div>
                            </div>

                        </div>
                    </div>
                </div>
            </div>
           
            <br>
            <h4 class="left light">Merged Pull Requests </h4>
            <div class="no-margin">
                <table class="padding-table">
                    <thead class="no-border">
                        <tr class="blue-grey-text text-lighten-2">
                            <td></td>
                            <td>Repository</td>
                            <td>Link to PRs</td>
                            <td>Description</td>
                        </tr>
                    </thead>
                    <tbody class="card activity">
                        {% for commits in page.activity %}
                        {% for c in commits %} 
                           <tr>
                                <td class="fl">{{ c[1][0]["repo"] | slice: 0 }}</td>
                                <td class="">&nbsp;{{ c[1][0]["repo"] }}</td>
                                <td><a href='{{ c[1][1]["link"] }}'>View</a></td>
                                <td>{{ c[1][2]["details"] | markdownify}}</td>
                           </tr>
                        {% endfor %}
                          
                        {% endfor %}
                    </tbody>

                </table>
  
            </div>
            <br>
            <div class="content card">
                <div class="card-content">
                    {{page.content  | markdownify }}
                </div>
            </div>
            <br><br>


		</div>
	</body>
</html> 

