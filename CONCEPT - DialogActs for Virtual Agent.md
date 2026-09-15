# DialogActs for Virtual Agent 

_As part of the Vancouver release, this feature expands Natural language Understanding (NLU) communication with Virtual Agent (VA), leading to more fluid conversations between user and agent._ 

## How DialogActs works 

DialogActs interprets and applies user inputs during a Virtual Agent conversation. With this feature active, you engage with the VA in your own natural language, instead of selecting replies based on prompts in the topic. 

For example, if you request a laptop in a VA conversation, you use the topic prompts to select a manufacturer, screen size, and amount of RAM. Without DialogActs, you change specifications only by following the prompts in the topic, potentially taking more time to loop through a VA conversation as you reset your options. With DialogActs, if you change your mind about any of the laptop's specifications before finishing the request, you can input an utterance such as, "Actually, add 8gb of RAM." If your input matches the NLU model closely enough, the specifications are changed immediately, even if you are on a different point in the topic. If the input does not match, it's added to a list of ignorable utterances. 
User utterances are stored in the _open_nlu_predict_state_tracking_ table, while feedback is tracked by the _open_nlu_predict_dialog_act_feedback_ table. Languages are tracked in the _open_nlu_driver_language_ table. 

As of the Vancouver release, English is the sole language support for DialogActs. 

## Activating DialogActs 

Activate DialogActs by toggling the Enable DialogActs switch in the Topic creation form or the Topic Properties tab. When activated, a second Confirm modified values toggle appears. Use this switch to provide prompts confirming when a variable is to be changed based on your utterances. 

## Considerations for implementing DialogActs 

No NLU model or associated intent is necessary for DialogActs to work. The feature is available as long as NLU is active for the instance and the topic. However, at least one of the preconfigured responses must be Active for the DialogActs toggles in the Topic Properties tab to be available. DialogActs can work without a model intent, but it cannot select an entity if the topic is not associated with that model or intent. 

Decision nodes can be modified by a condition or script to skip re-prompting by DialogActs. However, the Modify DialogActs toggle does not work if there are multiple date-time nodes on a topic. 

## Available DialogActs responses 

The Vancouver release includes the following types of responses, stored in the _)open_nlu_dialog_act_ table: 

### DialogActs response types 

| Type | Description |
| ----------- | ----------- |
| Modify | Alter a variable recorded previously. |
| Affirm | Confirm a variable. | 
| Negate | Decline confirming a variable. |

