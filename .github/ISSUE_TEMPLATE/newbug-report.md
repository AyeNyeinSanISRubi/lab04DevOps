name : Bug Report <br>
description : file a bug report <br>
title: "[Bug]:" <br>
labels: ["bug", "triage"] <br>
project: ["octo-org/1", "octo-org/44"] <br>
assiginees:
  - octocat 

body:
  - type: markdown <br>
    attributes: <br>
      value: | <br>
       			 Thanks for taking time to fill out this bug report.

   - type: input <br>
     id: contact <br>
     attributes: <br>
       label: Contact details<br>
       description: How can we keep in touch with you if we need more info?<br>
       placeholder: ex. @email.com <br>
     validations:<br>
       required: false<br>
	 - type: textarea<br>
     id: what-happened<br>
     attributes:<br>
     		label: What happened?<br>
    		description: Also tell us, what did you expect to happen?<br>
    		placeholder: Tell us what you see!<br>
    		value: "A bug happened!"<br>
    		validations:<br>
    				required: true
		- type: dropdown
                    id: version
                      attributes: 
             label: version
            description: What version of our software are you running?
             options:
                 - 1.0.2 (Default)
                 - 1.0.3 (Edge)
             default: 0
                        validations:
                            required: true
- type: dropdown
     id: browsers
          attributes:
               label: what browsers are you seeing the problem on?
               multiple: true
               options: 
                   - Firefox
                   - Chrome
                   - Safari
                   - Microsoft Edge
- type: textarea
     id: logs
     attributes: 
               label: Relevant log output
               description: Please copy and paste any relevant log output. This will be automatically formatted into code, so no need for backticks.
                Render: shell
- type: checkboxes
      Id: terms
      attributes: 
               label: Code of Conduct
               description: By submitting this issue, you agree to follow our [Code of Conduct] (https://example.com)
               options:
-              Label: I agree to follow this project’s Code of Conduct required: true
     
