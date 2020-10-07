# whyAPIs

# Taming the Shiny monolith

How do you know your Shiny app is too big? 
* hard to identify where to make changes 
* hard to pass off to new people or onboard new people 
* accidentally break it (one parenthesis off takes hours to fix) 


# Progression of a Shiny application
1. app.R file monolith
2a. get smarter and decouple UI from Server.  Organizational benefit only. 
2b. profile code (`profvis` and `shinyloadtest`)
3. Shiny modules
4. Tipping point -- hardened applications.  Web application. Shiny becomes a lightweight front end.  or it is recoded as a javascript front end. Focus is to put the brains in an API on the back end.   Decouple front end from processing with microprocessing. 
  Benefits are:
  a. maintainability
  b. reduction of technical debt
  c. sharability
  d. collaboration
  e. icing on the cake - side effects of focusing strictly on functionality

For each module, indentify processes and components that are important.  The connections are just httr requests to the API. 
