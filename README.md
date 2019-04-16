# steps to execute the application

1. Clone the project or download the zip.

2. Import the project as a maven project in the IDE

3. Jetty server plugin is added in the pom.xml so it can be executed using "mvn jetty:run"

4. This will start the jetty server on port-8080 (i.e. http://localhost:8080)

5. After opening the link http://localhost:8080 in the browser, put the below query and execute in order to fetch the data.

       {
         allLinks {
          url
          }
        }
        
6. Ececute the following mutation in order to create a link.

mutation createLink {
  createLink(url: "https://abc.com", description: "abc desc") {
    url
    description
  }
}


