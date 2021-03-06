- <script type="text/javascript" language="javascript">
        var aax_size='728x90';
        var aax_pubname = 'techpechu-21';
        var aax_src='302';
      </script>
      <script type="text/javascript" language="javascript" src="http://c.amazon-adsystem.com/aax2/assoc.js"></script>
- Overview
	- It's a private repository
	- Infinite storage space
	- Files inside repositories can be encrypted
	- Can be integrated with any pipeline tools like Jenkins
- #+BEGIN_WARNING
  Don't use root account to create ssh , always use non-root account
  #+END_WARNING
- Credential creation for Code Commit ->  [AWS Reference](https://docs.aws.amazon.com/codecommit/latest/userguide/setting-up-ssh-unixes.html) #hands-on
- Clone, Add , Commit , Push
	- Commands remains same as git : Refer -> [Basic Git commands](https://www.atlassian.com/git/glossary)
- Merging Strategies #exam-revise
  collapsed:: true
	- ![image.png](../assets/image_1647887484356_0.png)
	-
- Protect Master branch from unwanted commits #exam-revise
  collapsed:: true
	- To protect people from directly pushing changes to Master branch , we can restrict it with IAM policy [Guide to create IAM policy](https://docs.aws.amazon.com/codecommit/latest/userguide/how-to-conditional-branch.html) #hands-on
- Triggers and Notifications
  collapsed:: true
	- Code Commit supports both Triggers and Notifications
	- Notifications - are referred to [[SNS]]
	- Triggers - can be referred to [[SNS]] and [[Lambda]]
- [[CloudWatch events]]
  collapsed:: true
	- We can setup cloudwatch events configured based on Code Commit and can trigger multiple components like [[Lambda]] [[SNS]] [Refer here](https://docs.aws.amazon.com/codepipeline/latest/userguide/pipelines-trigger-source-repo-changes-console.html) #hands-on
- Code Commit as [[Lambda]] trigger 
  collapsed:: true
	- We can use Code Commit as Lambda trigger , so when ever a change occured on Code Commit Lambda can be executed [Refer here](https://docs.aws.amazon.com/codecommit/latest/userguide/how-to-notify-lambda.html) #hands-on