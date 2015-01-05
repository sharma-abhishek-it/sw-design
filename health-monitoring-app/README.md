# Health monitoring application - Software Requirements
### An application to view health status and report of a patient. It also alerts on emergency situations

-----------------------------------------

Detailed requirements

* A patient’s health should be monitored constantly
* On emergency situations an alert is sent to doctor and relative
* Patient & relative are added by doctor
* A scheduled report by Doctor is printed, as well as emailed to both doctor & relative
* Report schedule is configurable by doctor
* On demand report printing and/or report emailing is also present
* Health status consists of heartbeat, pulse rate plus other disease specific info like insulin ratio
* Status is viewable on mobile and patient equipment
* Monitoring should never go down but if it does an alert needs to be sent immediately to doctor
* Monitoring stopped message should also be shown on equipment
* Doctor should be able to view all patients with this equipment and a Good/Bad status in front of their names

------------------------------------------

Software Designer notes

* Later on more than one relative might be added for monitoring
* The might be relative(s) could be added by someone with adequate permissions
* Report schedule might be configurable independently for each observer
* Other mediums to display a report might be added later on
* Doctor might have grid view or list view of patients
* The setup might be extended to multiple doctors for a hospital
* Types of stakeholders(users) might increase e.g hospital, nurse, home caretaker etc.
