# RAM
RAM Class for automating Roblox Account Manager
Requirements:
AutoHotkey v2
Roblox Account Manager
Roblox Account Manager Settings:
Enable WebServer port:<port of your choice> 
Enable Every Request Requires PassWord
Enable Allow GetAccounts Method
Enable LaunchAccount Method
WebServerPass:<pass of your choice> Requires 6+ letters cannot contain symbols, letters and numbers only.


Example: 
RamInstance := RAM(8080 , "MyWebServerPass") ;Create Class with Port and WebServerPass
Accounts := RamInstance.GetAccountNames() ;Get all accounts names in ram as a Array
JobId := RamInstance.GetJobId(Accounts[1]) ;Get Jobid from Account 1 in ram
RamInstance.LaunchAccount(Accounts[1], JobId) ;Launch Account 1 with JobId from Ram
