# Season-Shot-Chart

*************************************************************************************
README FOR SCRAPING SEASON SHOT CHARTS
ANDRES GRANADA – ANDRESG1869@GMAIL.COM
ERIC DUPRE – EDUPRE7@LSU.EDU
*************************************************************************************
THIS PROGRAM WAS DEVELOPED WITH THE INTENTION OF SCRAPING AND PROCESSING AN ENTIRE SEASON’S WORTH OF SHOT CHART DATA FOR A COLLEGIATE 
BASKETBALL TEAM. AT THE END OF THE PROGRAM, YOU WILL HAVE A DATABASE OF ALL SHOTS TAKEN BY ALL MEMBERS OF A TEAM FOR AN ENTIRE SEASON.
THE DATA WE USE ARE SCRAPED FROM ESPN’S PLAY BY PLAY TAB OF A COLLEGIATE GAME, WHEN SHOT CHARTS ARE AVAILABLE. NOTE THAT SOME TEAMS DO
NOT HAVE SHOT CHARTS AVAILABLE FOR EVERY GAME WHILE OTHER TEAMS DO NOT HAVE SHOT CHART DATA AVAILABLE AT ALL. THIS PROGRAM IS ABLE TO 
IDENTIFY (AT THE GAME LEVEL) IF SHOT CHART DATA ARE AVAILABLE, BUT IT MAY BE MORE EFFICIENT FOR THE USER TO CHANGE THE PROGRAM IF DATA
IS ONLY AVAILABLE FOR NONE TO FEW GAMES INSTEAD OF HAVING THE PROGRAM SEARCH THROUGH THE ENTIRE SEASON.

NOW WE DISCUSS AN OVERVIEW OF THE PROCESSING AND LEAVE SPECIFIC DETAILS FOR COMMENTS WITHIN THE PROGRAM ITSELF. FOR THE PROGRAM TO 
RUN, THE USER ONLY NEEDS TO CHANGE WORKING DIRECTORY, TEAM NAME, AND THE TEAM’S HOME PAGE ON ESPN. THEN, THE PROGRAM OPENS A FIREFOX 
BROWSER WINDOW AND NAVIGATES TO THE TEAM’S PAGE. FROM THERE, THE PROGRAM COUNTS THE NUMBER OF GAMES ON THE SCHEDULE (FROM THE SCHEDULE
CHART ON THE LEFT OF THE PAGE). THEN, FOR EVERY GAME IN THE SEASON, THE PROGRAM NAVIGATES TO THE PLAY-BY-PLAY TAB AND IDENTIFIES IF 
THERE IS SHOT DATA. IF SUCH DATA IS AVAILABLE, THE PROGRAM SCRAPES THE DATA ON THE SHOT, IT’S LOCATION, WHO SHOT IT, ETC FOR EVERY 
SHOT FOR THE SPECIFIED TEAM.  NEXT, THE PROGRAM ITERATES THROUGH THE SAME PROCESS FOR EVERY GAME ON THE SCHEDULE, APPENDING ALL OF THE
SEASON’S SHOT CHART DATA IN ONE OBJECT, SHOTCHART. ONCE ALL OF THE DATA ARE COLLECTED, WE GO THROUGH A FEW CLEANING ROUTINES TO BREAK 
UP TEXT COLUMNS INTO MORE USEFUL COLUMNS. FINALLY, WE OUTPUT THIS DATA IN .CSV FORMAT AND PROVIDE A QUICK SHOT CHART EXAMPLE THAT CAN 
BE USED TO LAUNCH FURTHER PROJECTS. AS INDICATED ABOVE, THIS DATABASE CONTAINS DATA ON EVERY SHOT FROM EVERY PLAYER IN EVERY GAME, SO 
THE USER SHOULD DEVELOP PROCESSES TO CLEAN AND VISUALIZE THE DATA ACCORDING TO THEIR NEEDS. 

WE INTENDED TO MAKE OUR PROGRAM NIMBLE, SUCH THAT USERS ONLY NEED TO CHANGE 2-3 PARAMETERS TO SUCCESSFULLY RUN THIS ROUTINE FOR THEIR 
TEAM. IF THERE ARE ANY DIFFICULTIES RUNNING THIS SCRIPT OR IF THERE ARE ANY OTHER QUESTIONS/ CONCERNS, PLEASE FEEL FREE TO CONTACT 
EDUPRE7@LSU.EDU OR ANDRESG1869@GMAIL.COM. 
