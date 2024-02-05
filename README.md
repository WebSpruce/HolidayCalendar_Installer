[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/)
[![Version](https://img.shields.io/badge/version-v1.0.3-brightgreen.svg)](https://github.com/WebSpruce/HolidayCalendar_Installer/releases)

## 📸Holiday Calendar
<img src="https://github.com/WebSpruce/HolidayCalendar_Installer/blob/main/hc.gif?raw=true" height="400" alt="Holiday Calendar Screenshot"> | <img 

### 🗜️The solution structure

| Project | Features | Nugets |
| --- | --- | --- |
| `MAUI` | MVVM | CommunityToolkit.Maui, <br>CommunityToolkit.Mvvm, <br>Plugin.Maui.Calendar, <br>PublicHoliday
| `ASP API` | DTO, <br>Object Mapping, <br>Background Services, <br>Repository Pattern, <br>Dependency Injection |AutoMapper, <br> BCrypt.Net-Next, <br>FirebaseAuthentication.net
| `MODELS` |
| `SERVICES` | Repository Pattern |

### 📙Features

> [!IMPORTANT]
> The app is available on android and windows devices. <br>(_On windows device you have to install .NET 8.0 Runtime <a href="https://dotnet.microsoft.com/en-us/download/dotnet/8.0/runtime?cid=getdotnetcore&os=windows&arch=x64">you can install it from here</a> <br> (it also will show you information about it before installation)_)

The application is compatible with Android and Windows devices. 📱💻
Featuring both light and dark modes, the app dynamically adjusts based on the theme set on the device. 🌗

Each user is assigned a specific role within a group and branch. 👥🌐

From the homepage, users can efficiently submit new holiday requests, navigate to the calendar view, display a list of employees within their group, and review recently accepted events. In the calendar view, users can observe their approved holidays, view events related to their branch, or choose a specific branch. When a day is selected on the calendar, event information is displayed if there is an event scheduled for that day. 📅📆

The list of employees window facilitates the quick retrieval of contact information for colleagues. Administrators have the authority to approve or cancel the requests, edit user profiles, and adjust group settings as necessary. Within the group settings, administrators can find and regenerate join keys. Moreover, administrators have the ability to set the country for the calendar, displaying events for the entire year in the selected country. Additional functionalities include the capacity to add or remove branches. ⚙️🌍

The calculation of days off is based on whether the current date falls between October 1st and December 31st or between January 1st and September 30th. On an annual basis, users are provided with a default allocation of days off, and it is imperative to utilize any unused vacation days by September 30th, as they will be forfeited after that date. ⏰🗓️

**<a href="https://appetize.io/app/mwze3fwo4nlcbscx5ntg7qw2ve?device=pixel7&osVersion=13.0" target=”_blank” style="font-size: 20px; color:#99aab5 ;">--> ONLINE DEMO AVAILABLE HERE <--</a>**

### 📝Main Tasks

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
