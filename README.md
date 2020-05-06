# FlipFlop On-call Run Books

This project provides a guidance for Infrastructure Reliability Engineers and Managers who are starting an on-call shift or responding to an incident.
## On-Call

FlipFlop Reliability Engineers and Managers provide 24x7 on-call coverage to ensure incidents are responded to promptly and resolved as quickly as possible.

### Shifts

Shift assignments are available on the [Shift Schedule](https://docs.google.com/spreadsheets/d/1TORzWmN77Pz2XGc5gVzAUvynSY3PRPYu-Np5Wzcgkl0/edit#gid=0) 

## Checklists

### Shift Start
 - [ ] Log into the [production monitoring system](https://ff.prod.flipflopsystems.com/system/monitor/all)
 - [ ] Validate all monitor clocks are running if on-site
 - [ ] Check the latest asset request and make sure jobs are processing
 - [ ] Open the support ticketing queue
 - [ ] Sign in to slack and join the #production channel
 - [ ] Make sure your phone is on and not silent
 - [ ] Contact the current on-call engineer and relieve them before the end of their shift and start of yours.
 
### Shift End
 - [ ] Make sure you have closed any resolved issues, or pass them on to the next engineer
 - [ ] If you do not hear from the next on-call engineer by shift-end
    - [ ] Do not sign out, stay on-call
    - [ ] Call their listed number(s)
    - [ ] If you cannot reach them, call your engineering supervisor
 - [ ] Update the next engineer of any ongoing or recent issues
 

## Things to keep an eye on

### Calls

Answer the call concisely and professionally
- [ ] Engineering, this is _________.
- [ ] Collect and record
    - [ ] The issue
    - [ ] Scope of outage
    - [ ] Caller's station
    - [ ] Caller's name
    - [ ] Callers callback number

- If this is a severity 1 issue
    - [ ] I'll begin escalation of your issue. Someone will reach out if we need additional information.
    - [ ] End the call so you can begin the escalation checklist
    
- If this is NOT a severity 1 issue
    - [ ] Ask them to start a support ticket by emailing support@flipflopsystems.com
    
    

### Issues

First check on the status of any ongoing issues.

### Alerts

-   Check to make sure you have not received any system alerts
-   Check the support email queue for support requests
-   Check the reports queue for recent reports
-   Check the support call log

### Smoke Tests

-   Check how many pending jobs there are
-   Make sure you can access the [production app](https://ff.prod.flipflopsystems.com/)
-   Run an asset through "FF"

## Incidents

First: don't panic.

If you are feeling overwhelmed, escalate to the engineering manager.

## Communication Tools

If you do end up needing to post and update about an incident, we use [Statuspage](https://flipflop.statuspage.io/)

On Statuspage, you can [Make an incident](https://manage.statuspage.io/pages/mx4vtyyv3l4c/incidents).

Start by letting users know that we are investigating an issue until we have clear updates to provide.

Remember to close out the incident when the issue is resolved.  Also, when possible, put the issue and/or google doc in the post mortem link.

# Production Incidents

## Roles

During an incident all ops should monitor the #production slack channel

* On Call Engineer will
  * Call the director of engineering and communications manager [numbers](https://docs.google.com/document/d/1NtjL8SsT06IfKzjM5Ik-FyZMSJUGxHaojb94kqmExx8)
  * Open a war room on [meet](https://meet.google.com/_meet?pli=1&authuser=1) and post the url in #production slack.
  * Create a [Google Doc](https://drive.google.com/drive/u/1/folders/11bX1mFA8PiXiUcgvHXYYxSY5yJUljahD) to gather the timeline of events, share in #production
  * Redact the names to remove the blame. Only use team-member-1, -2, -3, etc.
  * Document partial findings or guessing as we learn.
  * Write a post mortem issue when the incident is solved.

* The communication manager will
  * Start and update an incident on [Statuspage](https://manage.statuspage.io/pages/mx4vtyyv3l4c/incidents).
  * Take over support calls and emails 
  * Escalate new issues or information to the on-call engineer
  
## General guidelines for production incidents.

* Is this an emergency incident?
	* Are we losing data?
	* Is prod.flipflopsystems.com down or serving a 504?
	* Has the incident affected users for greater than 1 hour?
	* Are all jobs failing?
	
* Emergency Incidents
    * Call the [director of engineering](https://docs.google.com/document/d/1NtjL8SsT06IfKzjM5Ik-FyZMSJUGxHaojb94kqmExx8)
    * Call the [communications manager ](https://docs.google.com/document/d/1NtjL8SsT06IfKzjM5Ik-FyZMSJUGxHaojb94kqmExx8)
    * Open a war room on [meet](https://meet.google.com/_meet?pli=1&authuser=1) and post the url in #production slack.
    * Create a [Google Doc](https://drive.google.com/drive/u/1/folders/11bX1mFA8PiXiUcgvHXYYxSY5yJUljahD) to gather the timeline of events, share in #production
	
* For non-emergency incidents.
	* Create a [Google Doc](https://drive.google.com/drive/u/1/folders/11bX1mFA8PiXiUcgvHXYYxSY5yJUljahD) to gather the timeline of events, share in #production
	* Email the [director of engineering](https://docs.google.com/document/d/1NtjL8SsT06IfKzjM5Ik-FyZMSJUGxHaojb94kqmExx8)

# But always remember!

Dont Panic!

