# AI Connector utility

_Use this utility to link generative AI to custom skills for added versatility in your Virtual Agent LLM (large language model) conversations._

## AI Connector utility properties

Specify the flow action properties for the node that you want to create.

| Property | Description |
| ----------- | ----------- |
| Node name | Name of the AI Connector node. |
| Select custom skill | Open the drop-down menu to search for a custom skill. | 
| Wait for response | Activate this toggle switch to wait for a response from the action before continuing the conversation. |
| **Input and Output mappings** |
| All input and output mappings are based on the custom skill you select. For more information on custom skills, see ***Now Assist SDK*** and ***Managing custom skills in Virtual Agent Designer***. |
| **Advanced** |
| Hide this node |
| Conditionally show this node if | No-code condition statement or low-code script that specifies a condition for presenting this node in the conversation. The condition must evaluate to true. |


## Example AI Connector utility controls 

| No skill selected | Skill selected |
| ----------- | ----------- |
| ![AI Connector utility with no skill selected. The utility functions only after you select a custom skill that includes a query.](https://github.com/TheIanCannon/TechAndWritingPortfolio/blob/main/portfolio%20images/AIConnector01.png)[_[AI Connector utility with no skill selected. The utility functions only after you select a custom skill that includes a query.]_] | ![AI Connector utility with Web Search skill selected. All input and output mappings derive from the custom skill.](https://github.com/TheIanCannon/TechAndWritingPortfolio/blob/main/portfolio%20images/AIConnector01.png)[_AI Connector utility with Web Search skill selected. All input and output mappings derive from the custom skill._] |
