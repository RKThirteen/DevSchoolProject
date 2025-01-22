# Final Project - Modified

Build an application from scratch which will contain backend implementation. The idea is to build a course management platform, which should have the following features:

The student should:
- Have the possibility to login – Use Spring Security and the password should not be saved in plaintext
- Be able to enrol to multiple courses
- Be able to see his enrolled courses and also the grades
- Not be able to enrol to multiple courses in the same time frame
- Not be able to enrol to a course that's already full

The user should:
- Have the possibility to login – Use Spring Security and the password should not be saved in plaintext
- Be able to create multiple courses: establish the schedule

Example of course creation Request: 
```json
{
	"name": "OOP",
	"description": "Oriented object programming basic",
	"maxAttendees": 30,
	"schedule": [
		{
			"name": "course",
			"startDate": "11.01.2023",
			"endDate": "01.06.2023",
			"weekDay": "MON",
			"startTime": "10:00",
			"endTime": "12:00"
		},
		{
			"name": "laboratory",
			"startDate": "11.01.2023",
			"endDate": "01.06.2023",
			"weekDay": "TUE",
			"startTime": "13:00",
			"endTime": "15:00"
		}
	]
}
```
- Be able to approve/deny student enrolment requests
- Be able to grade students: ONLY one grade per course per student

### Bonus
- use postman collection request chaining feature: pass a response parameter to the next request automatically instead of doing it manually
- test the business logic (the services)


