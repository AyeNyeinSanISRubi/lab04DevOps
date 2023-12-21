name : Bug Report   
description : file a bug report   
title: "[Bug]:"   
labels: ["bug", "triage"]   
project: ["octo-org/1", "octo-org/44"]   
assiginees:
  - octocat 

body:
  - type: markdown   
    attributes:    
      value: |     
    		Thanks for taking time to fill out this bug report.  

  - type: input   
    id: contact   
    attributes:   
       label: Contact details  
       description: How can we keep in touch with you if we need more info? 
       placeholder: ex. @email.com   
    validations:  
       required: false  
   - type: textarea  
     id: what-happened  
     attributes:    
     	label: What happened?  
    	description: Also tell us, what did you expect to happen?  
    	placeholder: Tell us what you see!  
    	value: "A bug happened!"  
     validations:  
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
	 - label: I agree to follow this project’s Code of Conduct     
 	   required: true     
     
