## **Schedule Automation System Summary**

This system is designed to automate the scheduling of employees based on their work preferences and availability.

**Features & Capabilities:**
1. **Data Management**: The system reads employee data from a CSV file, including names, date of hiring, availability days, preferred shift type, and preferred work location. 
2. **Database Handling**: A built-in database of sample employee data is provided, which can be saved and loaded as needed. The system checks for consistency in date format and sorts the data based on the date of hiring.
3. **User Interaction**: A user-friendly interface allows for manual modification of employee preferences using simple prompts.
4. **Advanced Scheduling Algorithm**: The system processes this data to create schedules that consider:
   - Employee availability.
   - Preferred work location.
   - Preferred shift type.
   - Maximum allowed employees per shift and location.
5. **Notification System**: Using the Twilio API, the system can send notifications to employees, informing them that the schedule for upcoming weeks has been posted.
6. **Date Calculations**: In-built functions allow the system to determine the upcoming Monday and a date three weeks from then.
7. **Readable Outputs**: The schedules for each location are tabulated and printed, offering clarity on day and swing shifts. A summary also highlights which employees need more shifts to meet the standard weekly criteria.

**Technical Aspects**:
   - Libraries used include pandas for data manipulation, tabulate for visually pleasing data presentation, Twilio for SMS notifications, and datetime for date calculations.

**Workflow**:
1. Data is loaded from a CSV or the sample database.
2. Users can modify employee preferences.
3. The system checks the database for consistency and sorts data.
4. The scheduling algorithm assigns shifts to employees, iterating over each employee, considering their preferences and availability, and avoiding over-scheduling.
5. Schedules for each location are tabulated and presented.
6. Employees can be notified of the new schedule via SMS notifications.

---
