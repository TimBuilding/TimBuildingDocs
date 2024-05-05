# Workflow

Learn how to perform a task or a series of tasks in a step-by-step manner.
Use the tools and resources provided to complete the task.

> **Pre-requisites**
>
> Make sure that you have completed the Getting Started guide.
>
{style="note"}

## Before you start

It is good practice to list the prerequisites that are required or recommended.

Make sure that:
- You have completed the Getting Started guide
- Have proper access to the required tools and resources

## How to perform a task

The tasks are broken down into steps to make it easier to follow.

1. Clone the repository to your local machine.

   ```bash
    gh repo clone <repository-name>
   ```

2. Read the requirements of the task. 

   ![Screenshot 2024-05-06 at 2.12.14 AM.png](Screenshot_2024-05-06_at_2.12.14 AM.png)

3. Change the status of the task to `In Progress`. 

   ![Screenshot 2024-05-06 at 2.13.22 AM.png](Screenshot_2024-05-06_at_2.13.22 AM.png)

4. Develop the feature or fix the bug.

5. Commit the changes to the repository.
   ```bash
   gt create -am 'Feature: Add new functionality'
   ```

6. Once you have completed the task. Commit the last changes and push them to the repository.
   ```bash
   gt create -am 'TIM-15 Feature: Finalized new functionality'
   gt submit
   ```
   > **Note!**
   > 
   > **TIM-15** is the task ID that you are working on.
   > Make sure to replace it with the actual task ID from Linear.app
   > ![Screenshot 2024-05-06 at 2.32.46 AM.png](Screenshot_2024-05-06_at_2.32.46 AM.png){style="block" width=200}
   > 
   {style="note"}

7. Add a description of the task, assign a reviewer and publish the task for review.

## Code Review

If your task requires a code review. 
It means that your code has been reviewed by a team member and feedback has been provided.
You have to make the necessary changes and resubmit the task for review.

1. Review the feedback provided by the reviewer.
   ![Screenshot 2024-05-06 at 2.55.30 AM.png](Screenshot_2024-05-06_at_2.55.30 AM.png){style="block" width=500}

2. Check out the branch that contains the changes.
   ```bash
   gt checkout
   ```
   Then select the branch that contains the changes.

3. Make the necessary changes to the code.

4. Commit the changes to the repository.
   ```bash
   gt modify
   ```

5. (Optional) If your code review requires you to fix conflicts, you can use the following command to resolve them.
   ```bash
   gt restack
   ```
   Fix the conflicts and then submit the changes.
   ```
   gt add -A
   gt continue
   ```

6. Once you have made the necessary changes, push them to the repository.
   ```bash
    gt submit
    ```
   
7. Mark the thread as resolved on Graphite.

8. Ask for a **Rerequest all reviews** from the reviewer through the Graphite app.
   ![Screenshot 2024-05-06 at 2.53.05 AM.png](Screenshot_2024-05-06_at_2.53.05 AM.png){style="block" width=500}