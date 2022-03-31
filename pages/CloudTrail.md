- CloudTrail by default records all events (any action performed by the user)that happens within your account
- Data events #exam-revise
  collapsed:: true
	- We can store all events in S3 or we can trigger [[Lambda]] for which we will be creating Trail and choose respective Data events
	- By default logs stored in S3 bucket are SSE-S3 encrypted
	- can be mapped to [[SNS]]  for every log file delivery
- CloudTrail Logs can be configured to get it delivered to [[CloudWatch Logs]]
- #+BEGIN_IMPORTANT
  #exam-revise 
  There is a 15 min delay for CloudTrail to S3 . If you need realtime notification then use [[CloudWatch events]] 
  #+END_IMPORTANT
- What info you can get from CloudTrail? #exam-revise
	- Who accessed?
	- What action been performed?
	- What was the response?
	- What role been used
- Log Integrity #exam-revise
	- What if someone modifies your logfiles to erase evidence?
		- With Log integrity api we can verify for
			- Modification or deletion of CloudTrail log files
			- Modification or deletion of CloudTrail digest files
			-