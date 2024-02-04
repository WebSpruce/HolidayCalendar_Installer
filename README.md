[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/)
[![Version](https://img.shields.io/badge/version-v1.0.3-brightgreen.svg)](https://github.com/WebSpruce/HolidayCalendar_Installer/releases)

### The solution structure

| Project | Features | Nugets |
| --- | --- | --- |
| `MAUI` | MVVM | CommunityToolkit.Maui, <br>CommunityToolkit.Mvvm, <br>Plugin.Maui.Calendar, <br>PublicHoliday
| `ASP API` | DTO, <br>Object Mapping, <br>Background Services, <br>Repository Pattern, <br>Dependency Injection |AutoMapper, <br> BCrypt.Net-Next, <br>FirebaseAuthentication.net
| `MODELS` |
| `SERVICES` | Repository Pattern |

### Features

> [!IMPORTANT]
> The app is on android and windows devices. <br>(_On windows device you have to install .NET 8.0 Runtime <a href="https://dotnet.microsoft.com/en-us/download/dotnet/8.0/runtime?cid=getdotnetcore&os=windows&arch=x64">you can install it from here</a> <br> (it also will show you information about it before installation)_)

The app is on Android and Windows devices.
The app has a light and dark mode depends of the theme set in the device

Every user has a role and is assigned to a group and branch.

From the homepage, you can quickly add a new request for holidays, go to the calendar view, display a list of employees from your group, and see recently accepted events.
In the calendar view, you can see your accepted holidays, your branch, or a selected branch.
When you select a day in the calendar, it shows event information if there is an event on that day.
You can quickly find contact information for your company’s friends in the list of employees window.
As an administrator, you can approve or cancel requests, edit users, and change group settings if needed.
In group settings, you can find and regenerate your join key. You are also able to set the country for your calendar (it shows events for the entire year in the selected country). Additionally, you can add or remove branches.

The number of days off is calculated based on whether the current date is between October 1st and December 31st or between January 1st and September 30th. Every year, you receive a default value of days off, and you must use your old vacation days by September 30th, unless they will be removed after that date.

**<a href="https://appetize.io/app/mwze3fwo4nlcbscx5ntg7qw2ve?device=pixel7&osVersion=13.0" target=”_blank” style="font-size: 20px; color:#99aab5 ;">--> ONLINE DEMO AVAILABLE HERE <--</a>**

<details>

<summary>Screenshots</summary>

| | | |
| --- | --- | --- |
| <img src="https://github.com/WebSpruce/HolidayCalendar_Installer/blob/main/HC_Screenshots/1.jpg?raw=true" height="400" alt="Holiday Calendar Screenshot"> | <img src="https://github.com/WebSpruce/HolidayCalendar_Installer/blob/main/HC_Screenshots/2.jpg?raw=true" height="400" alt="Holiday Calendar Screenshot"> | <img src="https://github.com/WebSpruce/HolidayCalendar_Installer/blob/main/HC_Screenshots/3.jpg?raw=true" height="400" alt="Holiday Calendar Screenshot">
| <img src="https://github.com/WebSpruce/HolidayCalendar_Installer/blob/main/HC_Screenshots/4.jpg?raw=true" height="400" alt="Holiday Calendar Screenshot"> | <img src="https://github.com/WebSpruce/HolidayCalendar_Installer/blob/main/HC_Screenshots/5.jpg?raw=true" height="400" alt="Holiday Calendar Screenshot"> | <img src="https://github.com/WebSpruce/HolidayCalendar_Installer/blob/main/HC_Screenshots/6.jpg?raw=true" height="400" alt="Holiday Calendar Screenshot">
| <img src="https://github.com/WebSpruce/HolidayCalendar_Installer/blob/main/HC_Screenshots/7.jpg?raw=true" height="400" alt="Holiday Calendar Screenshot"> |


</details>

### Main Tasks

- [x] The company has a unique join key, which can be changed in group settings.
- [x] The Calendar View shows accepted holidays for our company, our branch, or a selected branch. It displays events in the calendar with accepted status.
- [x] The amount of days off is always updated after accepting or rejecting the event.
- [x] There is a page with a list of our sent requests.
- [x] If you log in for the first time, you can choose to join an already existing group or create a new one.

Background Services in API:

- [x] The amount of days off is calculated for several years.
- [x] The system resets the amount of days off annually.
- [x] The amount of days off is updated every day.
- [x] Events with 0 attendees are removed.
- [x] User calendar events are removed if the user or calendar event doesn't exist.
- [x] The company ID is removed from the user if the company doesn't exist.
- [x] Firebase authentication has been implemented. 
