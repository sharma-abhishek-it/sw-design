## Architecture
* Entire ecosystem is based on server, mobile app(doctor & relatives) and embedded app(equipment)
* Fetching reports should be based on polling. Since no. of viewers per patient is very less, polling from clients is simple strategy
* We use mysql DB because of the nature of transactions - highly reliable data
* We make one app which serves both doctor & relative because of foll. reasons
  * In near future stakeholders might increase hence one app serves them all fits the model
  * Avoiding separate deployments for each type of user
  * If we make separate apps and later decide to switch to single, many customers will have to install new app
  * One drawback is that update to any type os user will trigger manual updates for all users
* Simple data viewing calls for a webapp(which is also faster to develop) rather than native app
* Choice of framework should be based on keeping codebase into one single place because:
  * Initial codebases should be more consolidated, and only as they grow should be divided into separate repos
  * If one language can serve all devices then use that framework for maximum code reuse
  * Build systems will use only code needed by the actual machine
  * Subsystems can always be split later on


## Software Design
