---
author_name: Céline Audin
author_profile: https://github.com/celineaudinsap
title: Run the Process with an Automation
description: Run the business process with a full monitoring of the workflow instances and automation jobs
auto_validation: true
time: 30
tags: [ tutorial>intermediate, software-product>sap-business-technology-platform, tutorial>free-tier]
primary_tag: software-product>sap-process-automation
---

## Prerequisites
 - Complete [Agent Management settings to execute the process with an automation](spa-run-agent-settings)
 - Complete [Configure Launchpad](spa-configure-launchpad)

## Details
### You will learn
  - How to run the Process
  - How to work on the Tasks
  - How to monitor Process and Automation
  - How to gain visibility into the Business Process
---

[ACCORDION-BEGIN [Step 1: ](Release and deploy the business process)]

You must first release and then deploy the business process project in order to run the process.

  !![Release](00_Release.png)

  !![Deploy](00_Deploy.png)

[DONE]
[ACCORDION-END]


[ACCORDION-BEGIN [Step 2: ](Run the business process)]

You will now run the process and learn how to monitor the process and work on the tasks. You have released and deployed the business process project.

1. From the deployed version of the Business Process Project in the **Overview** section, open the process **Order Processing**.

    !![Run](01_Open_Order_Processing.png)

2. Choose **Order Processing Form**.

3. Choose the **Copy** icon aside the **Form Link**.

    !![Run copy the form link](02_Process_Start.png)

4. Open the Form pasting the **Form Link** in a browser window.

    > When you open the form in the browser, you will see all the input fields you defined in the process trigger form.

5. Fill the form with the Customer Name and Order Number values and choose **Submit**.

    > You have to enter one of the order numbers from the excel file. Do not enter any random order number or else the automation will not give any results.

    !![Run open the form](Form_Inputs.png)

    After you choose the **Submit** button, you will receive a notification that the form has been successfully submitted.

6. The workflow has been triggered and the approval process has started. You can now work on the tasks, monitor the process and gain insights.

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 3: ](Work on the tasks)]

Tasks are requests for users to participate in an approval or review process. These tasks appear in the **My Inbox** application shipped with SAP Process Automation. Users can claim, approve, and/or reject the task from their inbox.

1. Start in the **Lobby** and open the **My Inbox** application by selecting the button ![Inbox Icon](02_Inbox_Icon.png) at the top right corner.

    !![Lobby](01_Lobby.png)

2. After opening the **My Inbox** application, you will see on the left-hand side all the tasks listed. Select the Approval Form, complete it and choose **Approve**.

    !![My Inbox Actions](03-MyInbox-Actions.png)

    > The provided tasks and forms might look different than this screenshot, depending on your configurations.

3. Depending on your selected actions and the information you have provided at the start of the process, the next task could be to **confirm** the order.

    Once you approve or reject the approval task, refresh the inbox again to get the final notification based on the action you took. Once you acknowledge the notification sent via the approval process, the process will be completed.

    !![Confirmation Form](06-ConfirmationForm.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 4: ](Monitor process and automation)]

Monitoring business processes is one of the key aspects of successful automation. Using monitoring capabilities, you can proactively and consistently monitor process performance, identify any issues in the process and take necessary actions to ensure business process continuity.

SAP Process Automation provides different applications for monitoring and managing different process skills. The applications include Process and Workflow Instances, Automation Jobs, Acquired Events etc. These applications are available under the **Monitor** tab in Application Development studio.

> All deployed processes can be accessed by following **Manage** > **Processes and Workflows application**.

1. To monitor all the running instances of the process, navigate to **Monitor** > **Process and Workflow Instances**.

    !![Monitor](01_Monitor.png)

    In there, you will see all the running, erroneous and suspended process instances. Use the filter bar to get a more customized view of the process instances based on different statuses such as running, completed, suspended, terminated, etc.

    To explore different process monitoring options, go to the **Instances** list and choose your new process instance that was just triggered via the start form.

2. Select your **Order Processing** instance to check the status of the **CONTEXT** and **EXECUTION LOG**.

    > Observe the process instance information, which provides the context for the process. You can see actual process data flowing across different activities in the process, and the execution logs where you can trace how the entire process has been progressing. You can also see some basic runtime information for each activity such activity name, who started it, when was it completed etc.

    !![Monitor](02-Process-and-Workflow.png)

3. Go to **Automation Jobs** under **Monitor**.

    !![Monitor](03_Automations_Jobs.png)

4. Choose the **Warning** icon (if applicable) to learn more about the Automation.

    > If this is the case, go to the [Settings](spa-run-agent-settings) section and add your agent in order to run the Automation Job.

    !![Monitor](03_Automations_Jobs_warning.png)

    You will see the automation ran successfully as below:

    !![Monitor](04_Monitor_Automation_successful.png)

    Notice the process instance progresses further to the approval step in the business process.

    !![Monitor](05-Monitor-Process-and-Workflow.png)

[VALIDATE_1]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 5: ](Gain visibility into the business process)]

You will need to configure your launchpad service. To do so, please [Configure your Launchpad](spa-configure-launchpad)

1. Navigate to the URL of the launchpad you configured.

2. Select **Process Workspace (Visibility Scenarios)**.

    !![Process Workspace](01_ProcessWorkspace.png)

3. **Search** for your visibility scenario and **select** it.

    !![Search Select](02-Search-Select.png)

4. The dashboard is there. The performance indicators are filling up, depending on the time it has taken, there might be different results. Please now feel free to explore the details and discover what is included in each tile.
You could even navigate into single instances.

    !![Browse Scenario](03_BrowseScenario.png)

[DONE]
[ACCORDION-END]




---
