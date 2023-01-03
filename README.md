📅 JS Calendar Library
License

Simple, lightweight, stylish calendar + organizer JavaScript Library

Installation — Basic Usage — Examples — Doc — Screenshots

🌏 Browser Support
Chrome Chrome	IE Internet Explorer	Edge Edge	Safari Safari	Firefox Firefox
Yes	10+	Yes	Yes	Yes
💾 Install
There are multiple ways to install the calendar library

Via CDN:
<head>
    <link href="https://cdn.rawgit.com/nizarmah/calendar-javascript-lib/master/calendarorganizer.min.css" rel="stylesheet" />
</head>

<body>
    <div id="calendarContainer"></div>
    <div id="organizerContainer"></div>

    <!-- Stick script at the end of the body -->
    <script src="https://cdn.rawgit.com/nizarmah/calendar-javascript-lib/master/calendarorganizer.min.js"></script>
    <script>
        /* Fill with whatever your dreams desire */
    </script>
</body>
Via download and self-hosting: Download the minified JavaScript file and minified CSS file
<!-- Insert in <head> -->
<link href="calendarorganizer.min.css" rel="stylesheet" />

<!-- Insert before you own <script> tag-->
<script src="calendarorganizer.min.js"></script>
🔨 Basic Usage
HTML
Place 2 <div>'s where you want the calendar to be placed

<body>
...
<div id="calendarContainer"></div>
<div id="organizerContainer"></div>
...
</body>
JavaScript
// Basic config
var calendar = new Calendar("calendarContainer", "small",
                            [ "Monday", 3 ],
                            [ "#ffc107", "#ffa000", "#ffffff", "#ffecb3" ],
                            {
                                days: [ "Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday",  "Saturday" ],
                                months: [ "January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December" ],
                                indicator: false,
                                placeholder: "<span>Custom Placeholder</span>"
                            });

var data = {
            2017: {
                12: {
                    25: [
                        {
                            startTime: "00:00",
                            endTime: "24:00",
                            text: "Christmas Day"
                        }
                    ]
                }
            }
        };

var organizer = new Organizer("organizerContainer", calendar, data);
Want to know how to customize your data? Check out the docs

