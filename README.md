1. Created ASP.NET MVC project
2. Using Angular CLI generated Angular project in the same folder(could be changed):
	ng new angular-app
3. In file .angular-cli.json changed where compiled files are exported
	outDir: "outDir": "../dist"
4. Added pre-build events for Asp.Net MVC:
	cd ../angular-app &
	ng build --base-href="/dist/" &
	cd ../bin
	