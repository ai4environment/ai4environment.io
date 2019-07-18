---
layout: page
title: Calendar
permalink: /calendar/
type: info
header_text: ai4environment
---
<!-- https://www.milanlund.com/blog/javascript-library-google-calendar -->

<script src="/assets/js/anchorme.min.js" type="text/javascript">
</script>
<script src="/assets/js/format-google-calendar.js" type="text/javascript">
</script>

<div class="span9">

<ul id="events-upcoming"></ul>
<ul id="events-past"></ul>

<!-- Step 3: Call the FormatGoogleCalendar -->
<script type="text/javascript">
formatGoogleCalendar.init({
 calendarUrl: 'https://www.googleapis.com/calendar/v3/calendars/ek23ehn48p1hd06353b0kvv7cg@group.calendar.google.com/events?key=AIzaSyCR3-ptjHE-_douJsn8o20oRwkxt-zHStY',
 past: false,
 upcoming: true,
 sameDayTimes: true,
 dayNames: true,
 pastTopN: -1,
 upcomingTopN: 10,
 itemsTagName: 'li',
 upcomingSelector: '#events-upcoming',
 pastSelector: '#events-past',
 recurringEvents: true, 
 upcomingHeading: '<p>Upcoming events (conferences, workshops, etc) in the field of AI for environmental science:</p>',
 pastHeading: '<h2>Past events</h2>',
 format: ['*date*', ': ', '*summary*', ' — ', '*description*', ' in ', '*location*'],
});
</script>

</div>

Want to add your event to the calendar? Drop us [an email](ai4enviroment@gmail.com)!
