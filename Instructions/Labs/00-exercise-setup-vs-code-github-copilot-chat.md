---
lab:
  title: Exercise - Set up Visual Studio Code with GitHub Copilot Chat
  module: Module 00 - Lab Environment Setup
  description: In this exercise, you install Visual Studio Code and the GitHub Copilot Chat extension, sign in with your GitHub account, and verify that the chat feature is working. Use these steps if you are setting up for the first time or if you have reinstalled Visual Studio Code.
  duration: 15 minutes
  level: 100
  islab: true
  primarytopics:
    - Visual Studio Code
    - GitHub Copilot
---

<!--
Edit the metadata above to manage the list of exercises in the home page of the GitHub site that gets generated.
You can delete the module and edit index.md in the root of the repo to customize the display so that only the exercises are listed
To enable GitHub page publishing, edit the Page settings for the repo and publish from the main branch
-->

# Set up Visual Studio Code with GitHub Copilot Chat <!-- match title in metadata above (and Learn Exercise unit and ILT slide)-->

In this exercise, you install Visual Studio Code and the GitHub Copilot Chat extension, sign in with your GitHub account, and verify that the chat feature is working.

> [!NOTE]
> Follow these steps whether you are setting up for the first time or if you have reinstalled Visual Studio Code. After a reinstall, extensions and sign-in sessions are not preserved and must be configured again.

This exercise should take approximately **15** minutes to complete.

> [!IMPORTANT]
> You will need a GitHub account with an active GitHub Copilot subscription (or a free trial) to complete this exercise.

## Task 1: Install Visual Studio Code

If you already have Visual Studio Code installed, skip to Task 2.

1. Open a browser and go to [https://code.visualstudio.com](https://code.visualstudio.com).
1. Select **Download for Windows** (or the appropriate option for your operating system).
1. Run the downloaded installer and follow the prompts, accepting the default options.
1. When installation is complete, open Visual Studio Code.

## Task 2: Install the GitHub Copilot and GitHub Copilot Chat extensions

After reinstalling Visual Studio Code, extensions are not automatically restored and must be reinstalled.

1. In Visual Studio Code, select the **Extensions** icon in the Activity Bar on the left side, or press **Ctrl+Shift+X** (Windows/Linux) or **Cmd+Shift+X** (macOS).
1. In the **Search Extensions in Marketplace** box, type `GitHub Copilot`.
1. Select **GitHub Copilot** from the results list and then select **Install**.
1. After the **GitHub Copilot** extension finishes installing, search for `GitHub Copilot Chat` in the Marketplace search box.
1. Select **GitHub Copilot Chat** from the results list and then select **Install**.

> [!NOTE]
> The **GitHub Copilot Chat** extension is separate from the core **GitHub Copilot** extension. Both must be installed and enabled for chat to work.

## Task 3: Sign in to GitHub

After reinstalling Visual Studio Code, you must sign in to GitHub again so that the extensions can access your Copilot subscription.

1. After the extensions are installed, Visual Studio Code may display a notification asking you to sign in to GitHub. If so, select **Sign In**.
1. If no notification appears, open the Command Palette by pressing **Ctrl+Shift+P** (Windows/Linux) or **Cmd+Shift+P** (macOS).
1. Type `GitHub Copilot: Sign In` and select that command from the list.
1. A browser window opens asking you to authorize Visual Studio Code to access your GitHub account. Select **Authorize Visual-Studio-Code**.
1. If prompted, enter your GitHub credentials and complete any two-factor authentication steps.
1. Return to Visual Studio Code. You should see a confirmation that you are signed in.

> [!TIP]
> You can verify your sign-in status by selecting the **Accounts** icon (person icon) in the Activity Bar. Your GitHub username should appear under the accounts list.

## Task 4: Verify GitHub Copilot Chat is working

1. In Visual Studio Code, open the GitHub Copilot Chat panel by selecting the **Chat** icon in the Activity Bar, or press **Ctrl+Alt+I** (Windows/Linux) or **Cmd+Option+I** (macOS).

   If you do not see the Chat icon, open the Command Palette (**Ctrl+Shift+P** or **Cmd+Shift+P**) and type `GitHub Copilot Chat: Open Chat` to open the panel.

1. In the chat input box, type a question such as `What is Azure?` and press **Enter**.
1. Verify that GitHub Copilot Chat returns a response.

If chat is working, you have successfully set up Visual Studio Code with GitHub Copilot Chat.

## Troubleshooting

If GitHub Copilot Chat is not responding after completing the steps above, try the following:

- **Check extension status**: In the Extensions view (**Ctrl+Shift+X**), verify that both **GitHub Copilot** and **GitHub Copilot Chat** show as **Enabled**. If either shows as disabled, select the extension and then select **Enable**.

- **Reload the window**: Open the Command Palette and type `Developer: Reload Window`, then press **Enter**. This restarts Visual Studio Code without closing it and can resolve extension activation issues.

- **Sign out and sign back in**: Open the Command Palette, type `GitHub Copilot: Sign Out`, press **Enter**, and then follow Task 3 again to sign back in.

- **Check your Copilot subscription**: Go to [https://github.com/settings/copilot](https://github.com/settings/copilot) in a browser and confirm that your GitHub Copilot subscription is active. If your subscription has expired, chat will not work.

- **Update extensions**: In the Extensions view, select the ellipsis menu (**...**) and then select **Check for Extension Updates**. Install any available updates for the GitHub Copilot extensions.

- **Reinstall the extensions**: In the Extensions view, right-click **GitHub Copilot Chat**, select **Uninstall**, and then follow Task 2 to reinstall.
