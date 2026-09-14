# Change the application scope for Virtual Agent Designer topics

_Set the application scope before you create or update a topic. For example, if you're creating IT Service Management (ITSM) topics, verify that you're in the **ITSM Virtual Agent Conversations** scope (and not the scope for the ITSM NLU (Natural Language Understanding) Model for Virtual Agent conversations)._

## **Before you begin**

Role required: virtual_agent_admin or admin

## **About this task**

When you open or create a topic, your current application scope displays in a status bar on the topic page. The status bar is visible in all tabs in your topic. If you open a topic not in your current scope, a warning banner appears on the canvas and you can’t edit the topic. You can still activate or deactivate, publish, or duplicate the topic. If you duplicate the topic, the duplicate sets to your current scope.

If you have multiple topics open at once, each topic shows its scope on all its tabs. All topics not set to the current scope are locked.

![Topic opened to canvas view in Virtual Agent Designer, with Application scope highlighted. The topic unlocks for editing when you change application scope to match the topic.](https://github.com/TheIanCannon/TechAndWritingPortfolio/blob/main/portfolio%20images/AppScopeChange.png)

## **Procedure**

1. In the unified navigation bar, select the Globe icon.

2. Select **Application Scope**, then choose the appropriate scope for your conversations. For example, select **Workflow Studio**.

### **Note:** If you're using domain separation, you can change the domain you're working in. Select **Domain scope: global** to change the domain. Any topics created within a domain are restricted to users of that domain. For more information, see _**Domain separation and Virtual Agent**_.

## **Result**

The application scope updates, and the new scope displays in the topic page when you refresh or open the topic. When the scope isn’t global, a ring appears around the globe icon (![Globe icon.](https://github.com/TheIanCannon/TechAndWritingPortfolio/blob/main/portfolio%20images/icon%20-%20globe.png)). 

If the new scope matches a topic that was locked before, the warning banner disappears, and you can edit the topic. 

## **What to do next**

Return to creating or updating your topic. If you have multiple topics open, you can slide the **Group tabs by app scope** toggle switch in Virtual Agent Designer settings to sort topics. For more information, see _**Virtual Agent Designer Topics page**_.

